# 绘制矢量图形

例：使用SVG绘制圆形、椭圆及动画

```javascript
<!DOCTYPE html>
<html>
<head lang="en">
<meta charset="UTF-8">
<title></title>
</head>
<body>
<svg width="120" height="120" viewBox="0 0 120 120" version="1.1">
<circle cx="60" cy="60" r="50"></circle>
</svg>
<svg width="120" height="120"
viewPort="0 0 120 120" version="1.1"
xmlns="http://www.w3.org/2000/svg">

<ellipse cx="60" cy="60" rx="50" ry="25"/>

</svg>

<svg width="120" height="120" viewBox="0 0 120 120"
xmlns="http://www.w3.org/2000/svg" version="1.1"
xmlns:xlink="http://www.w3.org/1999/xlink" >

<!-- Draw the outline of the motion path in grey, along
with 2 small circles at key points -->
<path d="M10,110 A120,120 -45 0,1 110 10 A120,120 -45 0,1 10,110"
stroke="lightgrey" stroke-width="2"
fill="none" id="theMotionPath"/>
<circle cx="10" cy="110" r="3" fill="lightgrey" />
<circle cx="110" cy="10" r="3" fill="lightgrey" />

<!-- Here is a red circle which will be moved along the motion path. -->
<circle cx="" cy="" r="5" fill="red">

<!-- Define the motion path animation -->
<animateMotion dur="6s" repeatCount="indefinite">
<mpath xlink:href="#theMotionPath"/>
</animateMotion>
</circle>
</svg>

<svg width="120" height="120"
viewPort="0 0 120 120" version="1.1"
xmlns="http://www.w3.org/2000/svg">

<rect x="10" y="10" width="100" height="100">
<animate attributeType="XML"
attributeName="x"
from="-100" to="120"
dur="10s"
repeatCount="indefinite"/>
</rect>

</svg>
</body>
</html>
```