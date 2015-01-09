# 标签及使用

## 标签

`<audio>` 定义声音

`<source>` 规定多媒体资源，可以是多个

## 控制器：control

control属性供添加播放、暂停、音量控件。

例：

```javascript
<!DOCTYPE HTML>
<html>
<body>
　<audio controls=“controls”>您的浏览器不支持
    <source src=“raw/1.mp3” type="audio/mpeg">
    <source src="raw/1.mp3" type="audio/ogg">
</audio>
</body>
</html>
```