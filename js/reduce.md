```
const numbers = [1, 2, 3, 4, 5];

// 使用 reduce 计算数组元素的总和
const sum = numbers.reduce((accumulator, currentValue) => {
  return accumulator + currentValue;
}, 0);

console.log(sum);
```


```
let res = { data: { list: [1, 2, 3] } }
let v = ['res', 'data', 'list'].reduce((acc, current) => {
    return acc?.[current]
}, { res })
console.log(v)
```