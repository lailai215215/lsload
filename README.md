# lsload
移动端 通过 localStorage 缓存 css 和 js 文件
## 使用方法

```
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8">
		<meta http-equiv="Pragma" content="no-cache">
		<meta http-equiv="Cache-Control" content="no-cache">
		<meta http-equiv="Expires" content="0">
		//设置html不进行缓存
		<script src="rem-dpr.min.js" type="text/javascript" charset="utf-8"></script>
		//移动端 rem 适配，详见https://github.com/Theoton/rem
	</head>

	<body>
		<script src="lsload.js" type="text/javascript" charset="utf-8"></script>
		<script type="text/javascript">
			//请按照加载顺序设置文件，更新版本请修改版本号 version
			var data =[
			{"name": "main","type": "css","version": "v1",url": "./css/main.css"},
			{"name": "index","type": "js","version": "v1","url": "./js/index.js"}
			];
			LS.load(data);
		</script>
	</body>
</html>
```
