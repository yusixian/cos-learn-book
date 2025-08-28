# 第三方库

{% embed url="https://infinum.com/blog/best-ios-libraries-2024/" %}

{% embed url="https://www.reddit.com/r/swift/comments/15oblcq/do_you_usually_use_rxswift_in_enterprise_projects/?tl=zh-hans" %}

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

慎用？

### SwiftLint

[SwiftLint](https://github.com/realm/SwiftLint) 一种实施快速风格和约定的工具，它基于现在存档的GitHub Swift样式指南。 Swiftlint强制执行 Swift 社区通常接受的样式指南规则。

### SnapKit

[https://github.com/SnapKit/SnapKit](https://github.com/SnapKit/SnapKit)

一个简单而有力的工具，用于定义约束，从而获得更好，更快和更快的发展。它的流利和表达语法提供了许多功能，包括锚定视图，简化纵横比以及其他高级功能。

{% embed url="https://github.com/SnapKit/SnapKit" %}

### Firebase

[https://github.com/firebase/firebase-ios-sdk](https://github.com/firebase/firebase-ios-sdk)

很难将 Firebase 称为库，因为它包含了一套工具，这些工具简化了应用程序开发的不同方面，例如身份验证，实时数据库，云存储，消息传递，分析，crashlytics等。

{% embed url="https://github.com/firebase/firebase-ios-sdk" %}

### KeychainAccess

[KeychainAccess](https://github.com/kishikawakatsumi/KeychainAccess) 简化与钥匙扣的交互。它提供了一组简单简便的API，用于存储，检索和管理安全信息。如果您想增强应用程序的安全性并保护其数据免受未经授权的访问，我们建议使用它。例如，您可以看到从钥匙扣中保存和获取密码有多容易。

### Lottie

[https://github.com/airbnb/lottie-ios](https://github.com/airbnb/lottie-ios)

知名 支持基于向量的动画，易于安装，跨平台兼容性，无需多言。

### Sourcery

[Sourcery](https://github.com/krzysztofzablocki/Sourcery) 是一种强大的代码生成工具，可以使用用户定义的模板自动重复任务。当您必须创建许多仅使用不同类名称的新测试文件时，这对于 mock 数据非常有用。

{% embed url="https://github.com/krzysztofzablocki/Sourcery" %}

### Charts

[Charts](https://github.com/ChartsOrg/Charts) 适用于 iOS/tvOS/OSX 的精美图表！跨平台 MPAndroidChart 的苹果版。

需注意的是 iOS 16，苹果已经发布了自己的图表版本

{% embed url="https://github.com/ChartsOrg/Charts" %}

### Kingfisher

[Kingfisher](https://github.com/onevcat/Kingfisher) 是我们常用的图片加载和缓存工具。您只需提供一个图片 URL 供该工具下载，它就会将图片发送到内存和磁盘缓存中，然后在许多 UIKit 友好类中显示出来。Kingfisher 还能帮助进行异步图片加载、占位符、过渡效果、处理等。它还支持 SwiftUI。

## 可能已经不需要了？

### Alamofire

[Alamofire](https://github.com/Alamofire/Alamofire) 曾经是 iOS 开发中最好、最常用的框架之一。它的主要任务是简化联网请求、处理响应、身份验证以及该工具提供的其他有用功能。

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

### Reactive programming

眼熟吧，但是 iOS 13+ [Combine](https://developer.apple.com/documentation/combine) 取代他了。

[Reactive programming](https://github.com/ReactiveX/RxSwift) 简单、优雅、功能强大。它旨在以 Observable 对象的形式实现异步操作和数据流的轻松组合。学习这种工作方式需要时间。

```swift
observable
 .subscribe(onNext: { // some action })
 .disposedBy(disposeBag)
 .disposedBy(disposeBag)
```
