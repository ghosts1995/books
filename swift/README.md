




---

字符串插值

贯穿
完备

解包

参数标签



---


?? -> `let informalGreeting = "Hi \(nickName ?? fullName)"` -> 和 kotlin 的 `?:` 空值合并运算符一样
?. -> `let res = foo?.abc()` -> 整个表达式的值也是一个可选值

..< -> 左闭右开
... -> 左闭右闭

try? -> `let res = try? foo.abc()` -> 如果函数抛出错误，该错误会被抛弃并且结果为 nil。否则，结果会是一个包含函数返回值的可选值。
