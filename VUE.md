# 关于Vue.js的笔记


#### v-show 和 v-if的使用时机
 - v-show:不管初始值，一定会加载，需要频繁切换时使用
 - v-if:初始值为false不加载，每次切换都会改变DOM，切换频率少时使用