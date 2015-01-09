# 表单属性：autocomplete

autocomplete 属性规定 form 或 input 域应该拥有自动完成功能。

当用户在自动完成域中开始输入时，浏览器应该在该域中显示填写的选项。

> 提示: autocomplete 属性有可能在 form元素中是开启的，而在input元素中是关闭的。
> 注意: autocomplete 适用于 <form> 标签，以及以下类型的 <input> 标签：text, search, url, telephone, email, password, datepickers, range 以及 color。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php" autocomplete="on">
First name:<input type="text" name="fname"><br>
Last name: <input type="text" name="lname"><br>
E-mail: <input type="email" name="email" autocomplete="off"><br>
<input type="submit">
</form>

<p>填写并提交表单，然后重新刷新页面查看如何自动填充内容。</p>
<p>注意 form的 autocomplete属性为 "on"（开），但是e-mail自动为“off”（关）。</p>

</body>
</html>
```