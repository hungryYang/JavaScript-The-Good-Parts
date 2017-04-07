## 与类相关的扩充
1. `getElementsByClassName()`
2. `classList`属性

    这个属性是新集合类型`DOMTokenList`梳理。与其他DOM集合类似，`DOMTokenList`也有一个`length`属性，取得每个元素也可以用`item()`或`[]`。此外还有一下方法：
    - `add()`：将给定的字符串值添加到列表中
    - `contains()`：表示列表中是否存在给定的值
    - `remove()`：从列表中删除给定的字符串
    - `toggle()`：如果列表中存在给定值则删除，如果不存在则添加。

    支持`classList`属性的有Firefox3.6+和Chrome

## 焦点管理
`document.activeElement`：引用DOM中当前获得了焦点的元素。获得焦点的方式有页面加载、用户输入、和在代码中调用`focus（）`方法.

`hasFocus()`检测文档是否获得了焦点。

## HTMLDocument的变化
1. readyState属性

Document的`readyState`属性有两个可能的值：
    - loading：正在加载的文档
    - complete：已经加载完文档

2. 兼容模式？？

3. head属性

## 字符集属性

`document.charset`：用来设定字符集

## 自定义数据类型
可以为元素添加非标准的属性，但要添加`data-`前缀。可以通过`dataset`属性设置自定义属性。

但是兼容性不好。

## 插入标记
1. innerHtml属性

    会像内部填充属性

2. outerHTLML属性

    会连带节点一起替换[JSBin](http://js.jirengu.com/pucaximuve/2/edit)

3. insertAdjacentHTML()方法

    接收两个参数：插入位置和要插入的HTML文本。

    - `beforebegin`：在当前元素之前插入一个紧邻的同辈元素。

    - `afterbegin`：在当前元素之下插入一个新的子元素或在第一个子元素之前在插入新的子元素

    - `beforeend`：在当前元素之下插入一个新的子元素或在最后一个子元素之后再插入新的子元素。

    - `afterend`：在当前元素之后插入一个紧邻的同辈元素。

## scrollIntoView()方法 ？？？






















