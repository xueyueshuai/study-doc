substring()、substr()、slice()
### 相同点
这三个方法都可以对字符串进行截取，并且返回一个新的字符串，也就是不会对原字符串进行修改

### 不同点
这三个方法的不同之处在于参数不同。
```
string.substring(start,stop)  // 都为正数
start	必需。一个非负的整数，开始位置(包含)。
stop	可选。一个非负的整数，结束位置(不包含)。如果省略，一直到字符串的结尾。

start 与 stop 相等，那么该方法返回的就是一个空串（即长度为 0 的字符串）。
如果 start 比 stop 大，那么该方法在提取子串之前会先交换这两个参数。
如果 start 和 stop 有负数，那么会把该参数自动转为0，然后继续上述规则。
```

```
string.substr(start,length)
start	必需。起始下标(可以正负)，如果是负数，那么该参数声明从字符串的尾部开始算起的位置。也就是说，-1 指字符串中最后一个字符，-2 指倒数第二个字符，以此类推。
length 可选。子串中的字符数。必须是数值。如果省略了该参数，那么返回从 string 的开始位置到结尾的字串。
```

```
string.slice(startIndex,endIndex)
startIndex ：指定从哪个索引位置开始提取子字符串。如果未指定，默认为0（即字符串的起始位置）。
endIndex：可选参数，指定提取子字符串的结束位置（不包括该位置的字符）。如果未指定，将提取到字符串的末尾。
startIndex 和 endIndex 可以是负数
```


```
string.substring(startIndex,stopIndex)  // 都为正数
string.substr(startIndex,length) // start 正负均可 length非负数
string.slice(startIndex,stopIndex) // 正负均可
```
