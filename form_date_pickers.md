# Input输入类型：Date Pickers（日期选择器）

HTML5 拥有多个可供选取日期和时间的新输入类型：

date - 选取日、月、年

month - 选取月、年

week - 选取周和年

time - 选取时间（小时和分钟）

datetime - 选取时间、日、月、年（UTC 时间）

datetime-local - 选取时间、日、月、年（本地时间）

例：

```javascript
<!DOCTYPE HTML>
<html>
<body>

<form action="/example/html5/demo_form.asp" method="get">
Date: <input type="date" name="user_date" />
<input type="submit" />
</form>

</body>
</html>
```