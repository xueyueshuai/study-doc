``` html

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>下载json文件</title>
</head>

<body>

<button onclick="onTest()">下载json文件</button>

<script>
  function onTest() {
    // 创建一个包含数据的 JSON 对象
    const jsonData = {
      name: "John Doe",
      age: 25,
      city: "Example City"
    };

    // 将 JSON 对象转换为字符串
    const jsonString = JSON.stringify(jsonData, null, 2); // 第二个参数是缩进空格数，用于更好的可读性

    // 创建一个 Blob 对象，该对象表示数据，并设置 MIME 类型为 application/json
    const blob = new Blob([jsonString], {type: "application/json"});

    // 创建一个下载链接
    const downloadLink = document.createElement("a");
    downloadLink.href = URL.createObjectURL(blob);
    downloadLink.download = "data.json"; // 设置文件名

    // 将下载链接添加到页面，并模拟点击触发下载
    document.body.appendChild(downloadLink);
    downloadLink.click();

    // 移除下载链接
    document.body.removeChild(downloadLink);
  }


</script>

</body>

</html>
```