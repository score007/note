# 关于DOM属性和方法的笔记


#### querySelectorAll和getElementsByClassName获取元素的区别
最大的区别就是querySelectorAll的实现类似于一组元素的快照，而并非对文档结构进行搜索的动态查询。所谓快照就是把某个时刻dom中的结构记录下来，而不是通过查询dom结构动态获取。这样实现可以避免使用NodeList对象通常会引起的大多数性能问题，但是也会带来新的问题，比如dom结构发生变化，这个选择器就无法使用了。



#### nodeType 属性返回节点类型。

 - 如果节点是一个元素节点，nodeType 属性返回 1。
 - 如果节点是属性节点, nodeType 属性返回 2。
 - 如果节点是一个文本节点，nodeType 属性返回 3。
 - 如果节点是一个注释节点，nodeType 属性返回 8。


