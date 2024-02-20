
# scrollIntoView 方法将调用它的元素滚动到浏览器窗口的可见区域
```
element.scrollIntoView（）; // 等同于element.scrollIntoView(true)
element.scrollIntoView（alignToTop）; //布尔参数
element.scrollIntoView（scrollIntoViewOptions）; //对象参数


scrollIntoViewOptions:
    behavior [可选]定义过渡动画。“auto”,“instant"或"smooth”。默认为"auto"。
    block [可选] “start”，“center”，“end"或"nearest”。默认为"center"。
    inline [可选] “start”，“center”，“end"或"nearest”。默认为"nearest"。
```
