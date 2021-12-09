## 页面导入样式时，使用link和@import有什么区别？

1. 从属性  
   1. link是html本身提供的标签，还可以设置rel，RSS等连接属性
   2. @import是css提供的语法规则
2. 加载顺序上
   1. link和dom一起加载
   2. @import等待页面加载完才被加载
3. 兼容性上
   1. link基本全部兼容，rel的stylesheet属性也全面兼容，其他则只有部分兼容
   2. @import是 CSS2.1 才有的语法，故只可在 IE5+ 才能识别
4. 可操作性上
   1. .link引用的css可以被js的Dom获取进行操作
   2. @import引用的css不能被Dom获取