# swiper
swiper 使用及源码分析


### Observer （监视器）的实现原理

**observer: false**

启动动态检查器(OB/观众/观看者)，当改变swiper的样式（例如隐藏/显示）或者修改swiper的子元素时，自动初始化swiper。
默认false，不开启，可以使用update()方法更新。

**observeParents: false**

将 observe 应用于 Swiper 的父元素。当Swiper的父元素变化时，例如window.resize，Swiper更新。

**实现原理**

(1) MutationObserver

(2) requestAnimationFrame
