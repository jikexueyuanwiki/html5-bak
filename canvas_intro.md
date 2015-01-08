# Canvas标签

## 概念

Canvas 对象表示一个 HTML 画布元素`<canvas>`。它没有自己的行为，但是定义了一个 API 支持脚本化客户端绘图操作。

你可以直接在该对象上指定宽度和高度，但是，其大多数功能都可以通过CanvasRenderingContext2D 对象获得。 这是通过 Canvas 对象的getContext() 方法并且把直接量字符串 "2d" 作为唯一的参数传递给它而获得的。

## Canvas的历史

这个 HTML 元素是为了客户端矢量图形而设计的。它自己没有行为，但却把一个绘图 API 展现给客户端 JavaScript 以使脚本能够把想绘制的东西都绘制到一块画布上。

`<canvas>` 标记由 Apple 在 Safari 1.3 Web 浏览器中引入。对 HTML 的这一根本扩展的原因在于，HTML 在 Safari 中的绘图能力也为 Mac OS X 桌面的 Dashboard 组件所使用，并且 Apple 希望有一种方式在 Dashboard 中支持脚本化的图形。

Firefox 1.5 和 Opera 9 都跟随了 Safari 的引领。这两个浏览器都支持 `<canvas>` 标记。

我们甚至可以在 IE 中使用 `<canvas>` 标记，并在 IE 的 VML 支持的基础上用开源的 JavaScript 代码（由 Google 发起）来构建兼容性的画布。
`<canvas>` 的标准化的努力由一个 Web 浏览器厂商的非正式协会在推进，目前 `<canvas>` 已经成为 HTML 5 草案中一个正式的标签。

## SVG 以及VML之间的差异

`<canvas>` 标记和 SVG 以及 VML 之间的一个重要的不同是，`<canvas>` 有一个基于 JavaScript 的绘图 API，而 SVG 和 VML 使用一个 XML 文档来描述绘图。

这两种方式在功能上是等同的，任何一种都可以用另一种来模拟。从表面上看，它们很不相同，可是，每一种都有强项和弱点。例如，SVG 绘图很容易编辑，只要从其描述中移除元素就行。

要从同一图形的一个`<canvas>` 标记中移除元素，往往需要擦掉绘图重新绘制它。