## 直接的父子组件通信

* props 和 $emit : 适用于直接的父子组件通信 : 
* this.$parent 和 this.$children : 

## 多层级父子组件

* $attrs 和 $listeners : 适用于和后代组件相互传达数据，如 A->B->C 在 A 和 C 之间通信
* provide 和 inject : 

## 兄弟组件

* bus : 适用于各种组件间的通信，父子，兄弟都可以；是事件总线型的
