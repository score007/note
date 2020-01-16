# 关于Canvas的学习笔记

#### canvas 替换内容
由于某些较老的浏览器（尤其是 IE9 之前的 IE 浏览器）或者浏览器不支持 HTML 元素 `<canvas>`，在这些浏览器上你应该总是能展示替代内容。
​支持` <canvas> `的浏览器会只渲染 `<canvas>` 标签，而忽略其中的替代内容。不支持` <canvas>` 的浏览器则 会直接渲染替代内容。


文本替换：
```
<canvas>
   你的浏览器不支持 canvas，请升级你的浏览器。
</canvas>
```
```
<canvas>
    <img src="./美女.jpg" alt=""> 
</canvas>
```