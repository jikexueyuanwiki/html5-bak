# sessionStroage

针对一个session的数据储存，当浏览器关闭，数据会被删除。

例：

```javascript
<!DOCTYPE HTML>
<html>
<body>

<script type="text/javascript">

sessionStorage.lastname="Potter";
document.write(sessionStorage.lastname);

</script>

</body>
</html>
```