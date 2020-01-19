# 关于CSS的学习笔记

#### reflow的原因：

1. 页面初始化的时候； 
2. 操作DOM时； 
3. 某些元素的尺寸变了； 
4. 如果 CSS 的属性发生变化了。

#### 减少 reflow/repaint

1. 不要一条一条地修改 DOM 的样式。与其这样，还不如预先定义好 css 的 class，然后修改 DOM 的 className。 
2. 不要把 DOM 结点的属性值放在一个循环里当成循环里的变量。 
3. 为动画的 HTML 元件使用 fixed 或 absoult 的 position，那么修改他们的 CSS 是不会 reflow 的。 
4. 千万不要使用 table 布局。因为可能很小的一个小改动会造成整个 table 的重新布局。