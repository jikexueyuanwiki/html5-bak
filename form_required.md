# 新的input属性：required

required 属性是一个 boolean 属性.

required 属性规定必须在提交之前填写输入域（不能为空）。

> 注:required 属性适用于以下类型的 `<input>` 标签：text, search, url, telephone, email, password, date pickers, number, checkbox, radio 以及 file。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
Username: <input type="text" name="usrname" required>
<input type="submit">
</form>

<p><strong>注意：</strong> Internet Explorer 9及更早IE版本，或Safari不支持input标签的 required 属性。</p>

</body>
</html>
```