## 1. 源码

```
@Composable
fun Card(
    modifier: Modifier = Modifier.None,
    shape: Shape = (+MaterialTheme.shapes()).card,
    color: Color = (+MaterialTheme.colors()).surface,
    border: Border? = null,
    elevation: Dp = 1.dp,
    children: @Composable() () -> Unit
) {
    Surface(
        modifier = modifier,
        shape = shape,
        color = color,
        elevation = elevation,
        border = border,
        children = children
    )
}
```

## 2. 使用

```
Card(elevation = Dp(1F), shape = RoundedCornerShape(Dp(4F))) {
}
```

---

MaterialTheme.shapes().card

* RoundedCornerShape
* CutCornerShape

* val CircleShape = RoundedCornerShape(50) // 圆角矩形的50%圆角就是圆了

---

> interface Shape --> abstract class CornerBasedShape --> data class RoundedCornerShape --> data class CutCornerShape

1. interface Shape

```
interface Shape {
    fun createOutline(size: PxSize, density: Density): Outline
}
```

2. abstract class CornerBasedShape

```
abstract class CornerBasedShape(
    private val topLeft: CornerSize,
    private val topRight: CornerSize,
    private val bottomRight: CornerSize,
    private val bottomLeft: CornerSize
) : Shape {
}
```

3. data class RoundedCornerShape

```
data class RoundedCornerShape(
    val topLeft: CornerSize,
    val topRight: CornerSize,
    val bottomRight: CornerSize,
    val bottomLeft: CornerSize
) : CornerBasedShape(topLeft, topRight, bottomRight, bottomLeft) {
}
```

4. data class CutCornerShape

```
data class CutCornerShape(
    val topLeft: CornerSize,
    val topRight: CornerSize,
    val bottomRight: CornerSize,
    val bottomLeft: CornerSize
) : CornerBasedShape(topLeft, topRight, bottomRight, bottomLeft) {
}
```

---

