# 新的input属性：min 和 max 

min、max 和 step 属性用于为包含数字或日期的 input 类型规定限定（约束）。

> 注: min、max 和 step 属性适用于以下类型的 `<input>` 标签：date pickers、number 以及 range。

例：

```javascript
<!DOCTYPE html>
<html>
<body>

<form action="demo-form.php">

输入 1980-01-01 之前的日期:
<input type="date" name="bday" max="1979-12-31"><br>

输入 2000-01-01 之后的日期:
<input type="date" name="bday" min="2000-01-02"><br>

数量 (在1和5之间):
<input type="number" name="quantity" min="1" max="5"><br>

<input type="submit">
</form>

<p><strong>注意:</strong> Internet Explorer 9及更早IE版本，Firefox不支持input标签的 max 和 min 属性。</p>
<p><strong>注意:</strong>
在Internet Explorer 10中max 和 min属性不支持输入日期和时间，IE 10 不支持这些输入类型。</p>

</body>
</html>
```
