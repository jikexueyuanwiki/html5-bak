# 新的input属性：formmethod

formmethod 属性定义了表单提交的方式，它覆盖了`<form>`元素的的method 属性。

>注: 该属性可以与 type="submit" 和 type="image" 配合使用。

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

<p><strong>注：</strong> Internet Explorer 9及更早IE版本不支持input标签的 formmethod 属性。</p>

</body>
</html>
```