# Input输入类型：number

number 类型用于应该包含数值的输入域。

你还能够设定对所接受的数字的限定：

例：

```javascript
<!DOCTYPE HTML>
<html>
<body>

<form action="/example/html5/demo_form.asp" method="get">
Points: <input type="number" name="points" min="1" max="10" />
<input type="submit" />
</form>

</body>
</html>
```

> 注：可用max、min、step、value来规定对数字类型的限定