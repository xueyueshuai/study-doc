```
    fetch('http://localhost:9408/api/demo/test5')
      .then(response => {
        return response.blob()
      })
      .then(blob => {
        // 创建一个 <a> 元素，设置下载链接
        let link = document.createElement('a');
        link.href = window.URL.createObjectURL(blob);
        link.download = blob.name || 'downloaded-file';

        // 添加 <a> 元素到文档，模拟点击以触发下载
        document.body.appendChild(link);
        link.click();

        // 移除 <a> 元素
        document.body.removeChild(link);
      })
      .catch(error => console.error('下载文件时出错:', error));
```