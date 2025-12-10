---
description: 自己总结的可能的最佳实践。
---

# 从 React 到 SwiftUI 的实践指南

## 开发环境配置

主要是 Xcode

```bash
# 安装 Xcode (仅 macOS)
xcode-select --install

# 验证 Swift 环境
swift --version

# 创建新 SwiftUI 项目
# 通过 Xcode → Create New Project → SwiftUI App
```

可使用 [Swift Online Compiler](https://swiftfiddle.com) 进行语法学习

待补充……

## React 与 Swift 对比

强烈推荐阅读 [swiftui-for-react-devs](https://github.com/unixzii/swiftui-for-react-devs) 的实践总结，结合官方文档与社区最佳实践。

### React vs SwiftUI 核心范式

| 特性    | React (JavaScript/TypeScript) | SwiftUI (Swift)        |
| ----- | ----------------------------- | ---------------------- |
| UI 范式 | 声明式 (JSX)                     | 声明式 (DSL)              |
| 状态管理  | useState/useReducer           | @State/@ObservedObject |
| 数据流   | Props/Context                 | @Binding/Environment   |
| 生命周期  | useEffect/useLayoutEffect     | .onAppear/.onDisappear |
| 类型系统  | 弱类型(JS)/强类型(TS)               | 强类型 + Optional         |
| 内存管理  | 垃圾回收                          | ARC + 值/引用类型           |

> **关键结论**：UI 层概念相似度超过 70%，但底层语言机制差异显著。建议采取"自上而下"学习路径：先掌握 SwiftUI 声明式语法，再深入 Swift 语言特性。

### 声明式 UI 转换实践

**React 组件**：

```javascript
function Welcome(props) {
  const [count, setCount] = useState(0);

  return (
    <div>
      <h1>Hello, {props.name}</h1>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

**等效 SwiftUI 实现**：

```swift
struct Welcome: View {
    let name: String
    @State private var count = 0
  
    var body: some View {
        VStack {
            Text("Hello, \(name)")
                .font(.title)
            Text("You clicked \(count) times")
            Button("Click me") {
                count += 1
            }
        }
    }
}
```

💡 **调试技巧**：使用 `#Preview` 宏实时预览 UI 变化，类似 React Hot Reload

```swift
#Preview {
    Welcome(name: "SwiftUI Developer")
}
```

### 状态管理迁移策略

| React 模式     | SwiftUI 等效方案           | 注意事项                |
| ------------ | ---------------------- | ------------------- |
| `useState`   | `@State`               | 仅用于当前视图的私有状态        |
| `useReducer` | `@State` + 自定义方法       | 或使用 `@Observable` 类 |
| Context API  | `@EnvironmentObject`   | 需要提前注入环境对象          |
| Redux        | `@Observable` + 共享状态容器 | 需要手动实现类似 Redux 的模式  |

**复杂状态管理示例**：

```swift
// 类似 React useReducer 的模式
class AppReducer: ObservableObject {
    @Published var state: AppState
  
    func dispatch(_ action: Action) {
        switch action {
        case .increment:
            state.count += 1
        case .decrement:
            state.count -= 1
        }
    }
}

struct ContentView: View {
    @StateObject private var reducer = AppReducer()
  
    var body: some View {
        VStack {
            Text("Count: \(reducer.state.count)")
            Button("Increment") {
                reducer.dispatch(.increment)
            }
        }
    }
}
```

### 网络请求与异步处理

**React 模式**：

```javascript
function UserProfile({ userId }) {
  const [user, setUser] = useState(null);
  const [loading, setLoading] = useState(false);

  useEffect(() => {
    const fetchUser = async () => {
      setLoading(true);
      try {
        const response = await fetch(`/api/users/${userId}`);
        setUser(await response.json());
      } catch (error) {
        console.error('Failed to fetch user:', error);
      } finally {
        setLoading(false);
      }
    };
  
    fetchUser();
  }, [userId]);

  if (loading) return <div>Loading...</div>;
  return <div>{user?.name}</div>;
}
```

**SwiftUI 实现**：

```swift
struct UserProfile: View {
    let userId: String
    @State private var user: User?
    @State private var isLoading = false
  
    var body: some View {
        Group {
            if isLoading {
                ProgressView()
            } else if let user {
                Text(user.name)
            } else {
                Text("User not found")
            }
        }
        .task {
            await loadUser()
        }
    }
  
    private func loadUser() async {
        isLoading = true
        defer { isLoading = false }
      
        do {
            let url = URL(string: "https://api.example.com/users/\(userId)")!
            let (data, _) = try await URLSession.shared.data(from: url)
            user = try JSONDecoder().decode(User.self, from: data)
        } catch {
            print("Failed to fetch user: \(error)")
        }
    }
}
```

\
⚠️ 常见错误：在非主线程更新 UI 状态💡 调试技巧：使用 `MainActor` 确保 UI 更新在主线程执行

```swift
@MainActor
func updateUserInterface() {
    // UI 更新代码
}
```

## 项目结构与工程化规范

[\[SwiftUI 100天\] WeSplit · 了解一个 SwiftUI 应用的基本结构](https://zhuanlan.zhihu.com/p/98342351) ｜ [英文原版](https://www.hackingwithswift.com/books/ios-swiftui/understanding-the-basic-structure-of-a-swiftui-app)

了解一个 SwiftUI 应用的基本结构当你创建一个 SwiftUI 应用时，你将得到一组总计 100 行左右代码的文件。大部分代码其实什么事也没做，只是占位符而已，你可以先忽略它们。随着你的推进，这些占位符的代码将会被修改。在 Xcode 中，你可能会在左边的空间看到这些文件，这个空间被称为 Project Navigator

* `AppDelegate.swift` 包含管理应用的代码。过去我们经常要在这里添加代码，不过现在已经很少需要这么做了。
* `SceneDelegate.swift` 包含启动应用窗口的代码。在 iPhone 上这个类做的事情不多，但是在 iPad 上，可能同一时间有几个应用打开，因此这个类很重要。
* `ContentView.swift` 包含程序 UI 的初始化代码，也是我们这个项目中所有工作展开的地方。
* `Assets.xcassets` 是一个 _asset catalog_ —— 应用中所有图片资源的集合。除了应用图标， iMessage 贴纸，你还可以在这里添加颜色。
* `LaunchScreen.storyboard` 是一个创建小块 UI 的视觉编辑器，这些 UI 会在应用启动时展示。
* `Info.plist` 是一个特殊值的集合。这些值向系统描述你的应用如何工作 —— 包括它的版本，支持的设备方向，等等。这些虽然不是代码，但也十分重要。
* `Preview Content` 是一个黄色的组，内部有 `Assets.xcassets`，这是另一个 _asset catalog_ ，向你展示程序运行时是长什么样。

项目中所有的工作都在 `ContentView.swift` 中展开

### **项目结构**

#### 主流 iOS 架构介绍

感觉，就用 MVC 或者 MVVM 吧， Model / View / Controller / Services 这样。

> 许多中小型应用程序，例如简单的天气或笔记应用程序，都利用 MVC 的简单性和直接性。数据模型、UI 视图和逻辑控制器的分离使应用程序易于理解。
>
> https://www.antino.com/blog/ios-app-architecture#blog-section-4

MVC

```
/MVC
├── /Model
│   ├── User.swift
│   ├── Article.swift
├── /View
│   ├── UserViewController.swift
│   ├── ArticleViewController.swift
├── /Controller
│   ├── UserController.swift
│   ├── ArticleController.swift
└── /Services
    ├── NetworkService.swift
```

\
参考 [Modern iOS Architecture Patterns and Best Practices](https://medium.com/@sharmapraveen91/modern-ios-architecture-patterns-and-best-practices-5320e2d9d1aa)

> 现代 iOS 架构模式与最佳实践主要包括 MVC、MVVM、Clean Architecture、VIPER、Redux/TCA 及响应式编程（RxSwift/Combine），强调关注点分离、可测试性、依赖注入、单向数据流与数据绑定等原则，并给出每种模式的典型目录结构及选型指南，帮助开发者按业务复杂度与可维护性需求选择合适方案。
>
>
>
> 1. 架构模式总览
>
> * 覆盖模型：MVC、MVVM、Clean Architecture、VIPER、Redux/TCA 与响应式编程实践。
> * 共同目标：关注点分离、可扩展、可测试、可维护，利用 Swift 与现代框架提升质量。
>
>
>
> 2. 模型-视图-视图模型（MVVM）
>
> * 核心：以 ViewModel 作为 View 与 Model 的中介，承载展示与转换逻辑。
> * 最佳实践：使用 Combine 或 RxSwift 数据绑定；业务逻辑不进 View；以单元测试验证 ViewModel。
> * 目录要点：Model / ViewModel / View 三层清晰，配套网络与数据抓取组件。<br>
>
> 3. Clean Architecture（洁净架构）
>
> * 分层：Entities（领域模型）、Use Cases/Interactors（业务用例）、Interface Adapters（适配与 ViewModel/Presenter）、Frameworks & Drivers（UI/网络/数据库）。
> * 最佳实践：严格分层与依赖方向控制；业务层可测试、与 UI 解耦；使用依赖注入（DI）。
> * 目录要点：实体、用例、适配器、外层框架与数据仓库分离。<br>
>
> 4. VIPER
>
> * 组件：View、Interactor、Presenter、Entity、Router 五部分，高内聚低耦合。
> * 最佳实践：导航交给 Router；Presenter 专注业务与格式化；各组件易于独立测试。
> * 目录要点：按角色模块化，服务与数据层独立。<br>
>
> 5. Redux / TCA（The Composable Architecture）
>
> * 核心概念：State、Action、Reducer、Store，单向数据流，状态不可变。
> * 最佳实践：逻辑可组合复用；通过对 Action/Reducer 的单元测试保证可预测性。
> * 目录要点：State/Action/Reducer/View/Store/Services 分层清晰。<br>
>
> 6. 模型-视图-控制器（MVC）
>
> * 特点：传统且常用，易于上手；易导致 Massive ViewController。
> * 最佳实践：用辅助对象或 ViewModel 分担控制器逻辑；用委托与协议降低耦合。
> *   目录要点：Model / View / Controller / Services 基本分层。
>
>
>
> 7. 响应式编程（RxSwift / Combine）
>
> * 价值：以声明式流处理用户输入、网络与异步事件。
> * 最佳实践：用 Observables（RxSwift）或 Publishers（Combine）绑定；UI 与业务职责分离；重视内存管理与订阅释放。<br>
>
> 8. 选型指南
>
> * MVC：小型或原型应用；快速实现基础功能。
> * MVVM：中等复杂度、需数据绑定与良好可测性。
> * Clean Architecture：大型、复杂业务，需高可维护与扩展性。
> * VIPER：多功能模块化应用，强调严格分层与可测试性。
> * TCA/Redux：复杂全局状态与频繁状态变更场景（如聊天、实时协作）。
> * 响应式编程：实时数据、复杂异步与事件驱动 UI。

**可能的文件夹类型详解**

在 Xcode 的 Project Navigator 中使用您的项目名称在组中将它们创建为 groups（黄色的小“文件夹”）。然后，对于每个组，通过打开右侧的文件检查器，点击灰色的小文件夹图标，然后在项目目录中使用组的名称创建一个新的子文件夹，将它们链接到项目路径中的实际目录。**命名规范**

* **文件名**: 使用 PascalCase，描述性名称
* **文件夹名**: 使用 PascalCase 或 camelCase
* **协议**: 以 "able" 或 "Protocol" 结尾
* **扩展文件**: 使用 "+" 连接，如 \`String+Validation.swift\`

#### 文件夹介绍

**App 文件夹**

**用途**: 应用程序的入口点和核心配置

* `AppDelegate.swift`: 应用程序生命周期管理（UIKit）
* `SceneDelegate.swift`: 场景生命周期管理（支持多窗口）
* `MyApp.swift`: SwiftUI 应用程序入口点

**最佳实践**:

* 保持这些文件简洁，避免业务逻辑
* 将复杂的初始化逻辑移到专门的服务类中

**Models 文件夹**

**用途**: 数据结构和模型定义

* 数据模型（如 User、Product）
* Core Data 实体
* API 响应模型
* 枚举类型

**组织建议**:

```
Models/
├── Core/
│   ├── User.swift
│   └── Product.swift
├── API/
│   ├── LoginResponse.swift
│   └── ProductListResponse.swift
├── Database/
│   └── UserEntity.swift
└── Enums/
    ├── UserType.swift
    └── OrderStatus.swift
```

**Views 文件夹**

**用途**: UI 组件和界面相关文件

* SwiftUI Views 或 UIKit ViewControllers
* 自定义 UI 组件
* 视图修饰器

**组织建议**:

```
Views/
├── Screens/
│   ├── Home/
│   │   ├── HomeView.swift
│   │   └── HomeDetailView.swift
│   └── Profile/
│       └── ProfileView.swift
├── Components/
│   ├── Buttons/
│   ├── TextFields/
│   └── Cards/
└── Modifiers/
    └── CustomModifiers.swift
```

**Services 文件夹**

**用途**: 业务服务和外部集成

* 网络请求服务
* 数据库操作
* 第三方 SDK 集成
* 缓存服务

**常见服务类型**:

```
Services/
├── Network/
│   ├── APIService.swift
│   ├── NetworkManager.swift
│   └── RequestInterceptor.swift
├── Storage/
│   ├── CoreDataService.swift
│   ├── KeychainService.swift
│   └── UserDefaultsService.swift
├── External/
│   ├── FirebaseService.swift
│   ├── AnalyticsService.swift
│   └── PushNotificationService.swift
└── Business/
    ├── AuthService.swift
    ├── PaymentService.swift
    └── LocationService.swift
```

**Utilities 文件夹**

**用途**: 通用工具和辅助功能

**Helpers 子文件夹**

通用帮助类：

```
Helpers/
├── ValidationHelper.swift
├── FormatterHelper.swift
├── CryptoHelper.swift
└── ImageHelper.swift
```

**Constants 子文件夹**

常量定义：

```
Constants/
├── AppConstants.swift
├── APIConstants.swift
├── UIConstants.swift
└── NotificationNames.swift
```

**Resources 文件夹**

**用途**: 应用程序资源文件

* 图片资源（Assets.xcassets）
* 字体文件
* 本地化字符串
* 配置文件

**Configuration 文件夹**

**用途**: 项目配置和构建设置

* Info.plist
* Entitlements
* xcconfig 文件
* 构建脚本

### 依赖管理（包管理）

Swift Package Manager （SPM）、CocoaPods 和 Carthage 是 iOS 开发生态系统中流行的三种依赖管理工具。其中 CocoaPods 已停止维护，现在基本上使用官方集成的 SPM - Swift Package manager

```swift
// swift-tools-version: 5.9
import PackageDescription

let package = Package(
    name: "MySwiftUIApp",
    platforms: [.iOS(.v17)],
    products: [
        .library(name: "MyApp", targets: ["MyApp"]),
    ],
    dependencies: [
        .package(url: "https://github.com/alamofire/alamofire.git", from: "5.8.0"),
    ],
    targets: [
        .target(
            name: "MyApp",
            dependencies: ["Alamofire"],
            path: "Sources",
            resources: [.process("Resources")]
        ),
    ]
)
```

然后是 [Tuist](https://docs.tuist.dev/en/)，就是现在使用的

* 大规模 iOS 项目管理
* 模块化和依赖管理
* 项目生成和配置

### 代码风格

Swift 社区存在多个被广泛认可的编码风格指南，其中最具影响力的包括 Apple 官方的 API 设计指南、Google 的 Swift 风格指南以及 Ray Wenderlich 的指南。这些指南的核心精神是一致的：避免冗余、避免歧义，并倾向于隐式而非显式，除非显式能够提升可读性。

* [Apple 官方的 API 设计指南](https://www.swift.org/documentation/api-design-guidelines/)
* [Google 的 Swift 风格指南](https://google.github.io/swift/)：很长，通过列出良好的编程实践，每一点都有充分的依据，这些实践通常是所有语言的基础。
* [Ray Wenderlich 的风格指南](https://github.com/kodecocodes/swift-style-guide)：清晰、一致和简短的既定目标。每条规则后面都有完整的解释、推理和一组该做和不该做的示例。
* [LinkedIn Swift code style](https://github.com/linkedin/swift-style-guide)：该指南主要侧重于代码格式化
* [Airbnb Swift Style Guide](https://github.com/airbnb/swift)：结构合理，规则解释准确。几乎每条规则都可以通过 SwiftLint 进行 lintable，该指南甚至提供了 Xcode 编辑器设置来满足格式部分的规则，这些规则可以很容易地应用于脚本。

以命名规范为例，Google 的风格指南明确推荐遵循 Apple 的 API 风格。一个经典的例子是，静态属性或类属性的命名不应以其类型名称为后缀，例如，不应命名为 `UIColor.redColor`，而应使用 `UIColor.red`。这一规则并非随心所欲，而是与 Swift 语言的设计哲学深度绑定。在这种情况下，类型名 `UIColor` 已经提供了足够的上下文信息，重复的 `Color` 后缀显得多余且嘈杂。类似的，一个遵循 Swift 惯例的 API 往往通过清晰的语法来表达其意图，例如，函数名中的介词（如 `with`、`to`）可以使调用代码读起来像一句自然语言的句子。为了在项目中强制执行这些规范，推荐使用像 SwiftLint 这样的自动化工具。

### 代码质量与自动化

1\. [**SwiftLint**](https://github.com/realm/SwiftLint)

* 代码风格检查和自动修复
* 可配置的规则集
* 集成到 Xcode 构建过程

2\. [**SwiftFormat**](https://github.com/nicklockwood/SwiftFormat)

* 自动代码格式化
* 统一团队代码风格

[SwiftLint](https://github.com/realm/SwiftLint) 是一个强制执行 Swift 编码风格和约定的强大工具。它能够自动检查代码中不符合规范的地方，如过长的行、强制解包等。通过将 SwiftLint 集成到 Xcode 的 `Build Phase` 中，开发者可以在每次构建时获得即时反馈，就像收到编译错误或警告一样。团队可以通过项目根目录下的 `.swiftlint.yml` 文件来统一配置规则，禁用或启用特定的检查，并为某些规则设置不同的严重级别（警告或错误）。

一个通用的 .swiftlint.yml 配置示例：

```yaml
disabled_rules:
- trailing_whitespace

opt_in_rules:
- empty_count
- empty_string

excluded:
- Carthage
- Pods
- SwiftLint/Common/3rdPartyLib

line_length:
    warning: 150
    error: 200
    ignores_function_declarations: true
    ignores_comments: true
    ignores_urls: true
    
function_body_length:
    warning: 300
    error: 500

function_parameter_count:
    warning: 6
    error: 8
    
type_body_length:
    warning: 300
    error: 500
    
file_length:
    warning: 1000
    error: 1500
    ignore_comment_only_lines: true
    
cyclomatic_complexity:
    warning: 15
    error: 25

reporter: "xcode"
```

**GitHub Actions CI 配置**：

```yaml
name: CI

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  build-and-test:
    runs-on: macos-latest
  
    steps:
    - uses: actions/checkout@v4
  
    - name: Select Xcode
      run: sudo xcode-select -switch /Applications/Xcode_15.0.app
  
    - name: Install SwiftLint
      run: brew install swiftlint
  
    - name: Lint Code
      run: swiftlint --strict
  
    - name: Build Project
      run: xcodebuild build -scheme MyApp -destination 'platform=iOS Simulator,name=iPhone 15'
  
    - name: Run Tests
      run: xcodebuild test -scheme MyApp -destination 'platform=iOS Simulator,name=iPhone 15'
```

### Swift DocC 文档

[DocC | Documentation](https://www.swift.org/documentation/docc/) DocC 是 Swift 的文档编译器，将基于 Markdown 的文档标记与指令编译为可预览、可托管的富文档，支持从源码注释生成 API 参考、撰写文章与构建交互式教程，并提供跨符号链接、术语定义、代码清单、表格与图片、页面结构分组和外观定制，以及面向多语言 API 的文档与分发流程。

## 扩展资源

* [官方的 5 hours 教程](https://developer.apple.com/tutorials/swiftui/)
* [SwiftUI 官方文档](https://developer.apple.com/documentation/swiftui/)
* [Swift 语言指南](https://docs.swift.org/swift-book/documentation/the-swift-programming-language/)
* [Apple 开发者论坛](https://developer.apple.com/forums/)
* [SwiftUI by Example](https://www.hackingwithswift.com/quick-start/swiftui)
* [GitHub - jogendra/example-ios-apps:  A curated list of Open Source example iOS apps developed in Swift. An amazing list for people who are beginners and learning ios development and for ios developers who need any example app or feature.](https://github.com/jogendra/example-ios-apps)
* [GitHub - vsouza/awesome-ios: A curated list of awesome iOS ecosystem, including Objective-C and Swift Projects](https://github.com/vsouza/awesome-ios)<br>
