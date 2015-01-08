# 新的input属性：formtarget

formtarget 属性指定一个名称或一个关键字来指明表单提交数据接收后的展示。

The formtarget 属性覆盖 `<form>`元素的target属性.

> 注: formtarget 属性与type="submit" 和 type="image"配合使用.

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
First name: <input type="text" name="fname"><br>
Last name: <input type="text" name="lname"><br>
<input type="submit" value="Submit as normal">
<input type="submit" formtarget="_blank" value="提交到一个新的页面上">
</form>

<p><strong>注意：</strong> Internet Explorer 9及更早IE版本不支持input标签的 formtarget 属性。</p>

</body>
</html>
```