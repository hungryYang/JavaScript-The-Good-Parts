`instanceof` 运算符用来测试一个对象在其原型链中是否存在一个构造函数的 prototype 属性。

如果表达式 obj instanceof Foo 返回true，则并不意味着该表达式会永远返回true，因为Foo.prototype属性的值有可能会改变，改变之后的值很有可能不存在于obj的原型链上，这时原表达式的值就会成为false。

## instanceof和多全局对象(多个frame或多个window之间的交互)
在浏览器中，我们的脚本可能需要在多个窗口之间进行交互。多个窗口意味着多个全局环境，不同的全局环境拥有不同的全局对象，从而拥有不同的内置类型构造函数。这可能会引发一些问题。比如，表达式 `[] instanceof window.frames[0].Array` 会返回false，因为 `Array.prototype !== window.frames[0].Array.prototype`


