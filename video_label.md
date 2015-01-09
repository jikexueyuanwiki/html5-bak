# 标签及使用

## 标签

`<video>` 定义声音
`<source>` 规定多媒体资源，可以是多个

## 属性

width：宽
height：高

## 控制器：control

control属性供添加播放、暂停、音量控件。

例：

```javascript
<!DOCTYPE HTML>
<html>
<body>
　<video controls=“controls”>
　　<source src=“raw/1.mp4” >
　　<source src="raw/1.ogg" >
您的浏览器不支持</video>
</body>
</html>
```
