```
fetch('http://localhost:3000/books', {
    method: 'post',
    body: JSON.stringify({
        uname: '张三',
        pwd: '456'
    }),
    headers: {
        'Content-Type': 'application/json' // 这个很重要 post传参 要这一行
    }
}).then((response) =>{
    if (!response.ok) {
        throw new Error('网络响应不正常');
    }
    return response.json(); // 从响应中解析 JSON 数据
}).then( (res)=> {
    console.log(res)
});


```