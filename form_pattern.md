# 新的input属性：pattern

pattern 属性描述了一个正则表达式用于验证 `<input>` 元素的值。

> 注:pattern 属性适用于以下类型的 `<input>` 标签: text, search, url, tel, email, 和 password.

> 提示： 是用来全局 title 属性描述了模式.

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">
Country code: <input type="text" name="country_code" pattern="[A-Za-z]{3}" title="Three letter country code">
<input type="submit">
</form>

<p><strong>注意:</strong> Internet Explorer 9及更早IE版本，或Safari不支持input标签的 pattern 属性。</p>

</body>
</html>
```