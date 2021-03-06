数组在 Kotlin 中使用 Array 类来表示。

* 使用 [] 语法
* 有 size 属性

---

我们可以使用库函数 arrayOf() 来创建一个数组并传递元素值给它，这样 arrayOf(1, 2, 3) 创建了 array [1, 2, 3]。 或者，库函数 arrayOfNulls() 可以用于创建一个指定大小的、所有元素都为空的数组。

---

Kotlin 也有无装箱开销的专门的类来表示原生类型数组: ByteArray、 ShortArray、IntArray 等等。这些类与 Array 并没有继承关系，但是它们有同样的方法属性集。它们也都有相应的工厂方法:

ByteArray byteArrayOf
ShortArray shortArrayOf
IntArray intArrayOf
LongArray longArrayOf

```
val x: IntArray = intArrayOf(1, 2, 3)
x[0] = x[1] + x[2]
```

---



