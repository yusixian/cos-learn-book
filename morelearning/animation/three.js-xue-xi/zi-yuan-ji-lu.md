---
description: 记录一些用到的插件/资源
---

# 资源记录

## 资源网站

### Textures

[Poliigon](https://www.poliigon.com/) 是一个提供高质量3D资源的网站，旨在帮助艺术家和设计师创建更加真实的3D渲染作品。该网站提供成千上万的纹理、模型和高动态范围图像（HDRIs），这些资源都经过专业设计，适用于建筑可视化、产品渲染、游戏设计、视觉特效和动画制作。用户可以找到各种材质纹理，如砖块、混凝土、木材、金属等，以及各类模型和环境HDRIs​​。

{% embed url="https://www.poliigon.com/" %}
[https://www.poliigon.com/](https://www.poliigon.com/)
{% endembed %}

[3D Textures](https://3dtextures.me/) 提供免费的无缝PBR（物理基于渲染）纹理，包括漫反射、法线、位移、环境遮挡和粗糙度贴图。这些纹理适用于3D模型和场景的渲染，可帮助增强作品的真实感和视觉效果。网站上的纹理多样，适用于各种3D渲染项目​​。

{% embed url="https://3dtextures.me/" %}
[https://3dtextures.me/](https://3dtextures.me/)
{% endembed %}

[Arroway Textures ](https://www.arroway-textures.ch/) 是一家专门生产高质量数字纹理的公司，这些纹理适用于3D渲染和实时使用。他们坚信最好的纹理来源于现实物理世界，因此开发了自己的定制硬件和软件，以捕捉自然材料比单纯颜色更多的信息。Arroway Textures 提供的纹理对于提高3D作品的真实感和细节表现至关重要​​。

{% embed url="https://www.arroway-textures.ch/" %}
[https://www.arroway-textures.ch/](https://www.arroway-textures.ch/)
{% endembed %}

[Poly Haven](https://polyhaven.com/hdris) 是一个公共3D资源库。它提供一系列资源，包括 HDRI（高动态范围图像）、纹理和模型。这些资源通常用于 3D 建模、渲染和图形设计。 Poly Haven 根据免费使用许可提供这些资产，使其成为数字艺术家和设计师的宝贵资源​​。

{% embed url="https://polyhaven.com/hdris" %}
[https://polyhaven.com/hdris](https://polyhaven.com/hdris)
{% endembed %}

[M**atcaps**](https://github.com/nidorx/matcaps) 提供了一个庞大的MatCap（材质捕捉）纹理库。这些纹理以PNG和ZMT格式提供，专门用于3D计算机图形中，用于创建高质量的视觉效果。MatCap技术能够简化3D对象的视觉呈现，尤其是在雕塑和非真实感图像渲染中非常有用，因为它可以通过单个纹理实现复杂的材质和光照效果

{% embed url="https://github.com/nidorx/matcaps" %}

## vscode 插件

### WebGL GLSL Editor

[WebGL GLSL Editor](https://marketplace.visualstudio.com/items?itemName=raczzalan.webgl-glsl-editor) 是一个用于Visual Studio Code的扩展，它提供了对WebGL GLSL着色器的语言支持。这个扩展支持GLSL ES 100（WebGL 1 和 OpenGL ES 1.00）和GLSL ES 300（WebGL 2 和 OpenGL ES 3.00），以及所有兼容WebGL的GLSL扩展。它支持大多数众所周知的VS Code语言功能，如语法高亮、智能提示等。这个扩展是为使用WebGL进行3D图形开发的开发者设计的，可以极大地提高编写和调试GLSL着色器的效率​​。

{% embed url="https://marketplace.visualstudio.com/items?itemName=raczzalan.webgl-glsl-editor" %}
[https://marketplace.visualstudio.com/items?itemName=raczzalan.webgl-glsl-editor](https://marketplace.visualstudio.com/items?itemName=raczzalan.webgl-glsl-editor)
{% endembed %}

### Shader languages support for VS Code

[Shader languages support for VS Code](https://marketplace.visualstudio.com/items?itemName=slevesque.shader) 是另一个Visual Studio Code扩展，它提供了对多种着色器语言的支持。该扩展支持的着色器语言包括HLSL（High-Level Shading Language）、GLSL（OpenGL Shading Language）和Cg（C for Graphics）。这个扩展的主要特点是为这些着色器语言提供语法高亮功能。它对于游戏开发、图形设计和3D渲染等领域中使用着色器语言的开发者来说非常有用，可以帮助他们更轻松地编写和管理着色器代码

{% embed url="https://marketplace.visualstudio.com/items?itemName=slevesque.shader" %}
[https://marketplace.visualstudio.com/items?itemName=slevesque.shader](https://marketplace.visualstudio.com/items?itemName=slevesque.shader)
{% endembed %}

## Tips

### 画布与分辨率设置

{% embed url="https://juejin.cn/post/7101207945387442212" %}

* **画布充满窗口**：使用`window.innerWidth`和`window.innerHeight`属性来设置画布尺寸，使之充满整个浏览器窗口，并建议移除canvas标签上的宽高设置​​。
* **处理窗口调整**：文章中解释了如何监听resize事件，以便在窗口尺寸变化时更新画布尺寸、相机的视角比例和渲染器的大小​​。&#x20;
* **像素比问题**：讨论了如何处理屏幕上的锯齿问题，通过设置`renderer.setPixelRatio()`来调整像素比，推荐最大值设为2以兼顾性能​​。

```javascript
renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2))
// resize
window.addEventListener('resize', () => {
  // update sizes
  sizes.width = window.innerWidth
  sizes.height = window.innerHeight

  // update camera
  camera.aspect = sizes.width / sizes.height
  camera.updateProjectionMatrix()

  // update renderer
  renderer.setSize(sizes.width, sizes.height)
+  renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2))
})
```

* **全屏功能**：介绍了如何监听双击事件来实现全屏切换功能，并考虑到了 Safari 浏览器兼容

```javascript
window.addEventListener('dblclick', () => {
  const fullscreenElement = document.fullscreenElement || document.webkitFullscreenElement
  if (fullscreenElement) {
    if (document.exitFullscreen) {
      document.exitFullscreen()
    } else {
      document.webkitExitFullscreen()
    }
  } else {
    if (canvas.requestFullscreen) {
      canvas.requestFullscreen()
    } else {
      canvas.webkitRequestFullscreen()
    }
  }
})

```

