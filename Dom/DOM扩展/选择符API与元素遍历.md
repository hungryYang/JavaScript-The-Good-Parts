## 选择符API
1. `querySelector()`
2. `querySelectorAll()`

## 元素遍历
对于元素的空格IE9及之前版本不会返回文本节点，而其他所有浏览器都会返回文本节点。新增了一组属性来弥补差异：

- `childElementCount`：返回子元素的个数
- `firstElementChild`：指向第一个子元素；firstChild元素版
- `lastElementChild`
- `previousElementSibling`
- `nextElementSibling`
