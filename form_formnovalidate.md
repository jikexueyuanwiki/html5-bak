# 新的input属性：formnovalidate

novalidate 属性是一个 boolean 属性，它描述了 <input> 元素在表单提交时无需被验证。

formnovalidate 属性会覆盖 <form> 元素的novalidate属性.

> 注: formnovalidate 属性与type="submit一起使用

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php" method="get">
First name: <input type="text" name="fname"><br>
Last name: <input type="text" name="lname"><br>
<input type="submit" value="Submit">
<input type="submit" formmethod="post" formaction="demo-post.php" value="Submit using POST">
</form>

<p><strong>注意：</strong> Internet Explorer 9及更早IE版本不支持input标签的 formmethod 属性。</p>

</body>
</html>
```