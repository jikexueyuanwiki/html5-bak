# 新的input属性：autofocus

autofocus 属性是一个 boolean 属性，规定在页面加载时，域自动地获得焦点。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
First name: <input type="text" name="fname" autofocus><br>
Last name: <input type="text" name="lname"><br>
<input type="submit">
</form>
<p><strong>注意：</strong> Internet Explorer 9及更早IE版本不支持input标签的 autofocus 属性。</p>

</body>
</html>
```