```
Array(10).fill(0) // [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
Array(10).fill(0).map((v,k)=>k) // [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```
```
Array.from(Array(10)) // [undefined, undefined, undefined, undefined, undefined, undefined, undefined, undefined, undefined, undefined]
Object.keys(Array.from(Array(10))) // ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
```