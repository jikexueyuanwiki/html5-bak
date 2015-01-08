# 新的input属性：placeholder

placeholder 属性提供一种提示（hint），描述输入域所期待的值。
简短的提示在用户输入值前会显示在输入域上。

> 注: placeholder 属性适用于以下类型的 `<input>` 标签：text, search, url, telephone, email 以及 password。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
<input type="text" name="fname" placeholder="First name"><br>
<input type="text" name="lname" placeholder="Last name"><br>
<input type="submit" value="Submit">
</form

<p><strong>注意：</strong> Internet Explorer 9及更早IE版本不支持input标签的 placeholder 属性。</p>

</body>
</html>
```