# 使用Geolocation API

## 介绍

用于获得用户的地理位置。

> 注：鉴于该特性可能侵犯用户的隐私，除非用户同意，否则用户位置信息是不可用的。

## 浏览器支持

Internet Explorer 9、Firefox、Chrome、Safari 以及 Opera 支
持地理定位。

> 注：对于拥有 GPS 的设备，比如 iPhone，地理定位更加精确。


## 运行原理

判断浏览器是否支持Geolocation

如果支持，则运行 getCurrentPosition() 方法。如果不支持，则向用户
显示一段消息。

例：

```javascript
<!DOCTYPE html>
<html>
<body>
<p id="demo">点击这个按钮，获得您的坐标：</p>
<button onclick="getLocation()">试一下</button>
<script>
var x=document.getElementById("demo");
function getLocation()
{
if (navigator.geolocation)
{
navigator.geolocation.getCurrentPosition(showPosition,showError);
}
else{x.innerHTML="Geolocation is not supported by this browser.";}
}
function showPosition(position)
{
x.innerHTML="Latitude: " + position.coords.latitude +
"<br />Longitude: " + position.coords.longitude;
}
function showError(error)
{
switch(error.code)
{
case error.PERMISSION_DENIED:
x.innerHTML="User denied the request for Geolocation."
break;
case error.POSITION_UNAVAILABLE:
x.innerHTML="Location information is unavailable."
break;
case error.TIMEOUT:
x.innerHTML="The request to get user location timed out."
break;
case error.UNKNOWN_ERROR:
x.innerHTML="An unknown error occurred."
break;
}
}
</script>
</body>
</html>
```