### 动画的理解
```
html原生动画效果分为两类：过渡和动画。
过渡效果是利用transition结合伪类class:hover；
动画效果就是自定义好动画后，最后用animation去使用该效果。
vue动画就是它自己创建了个<transition></transition>标签，定义好动画相关的样式类：

.v-enter-from 
.v-enter-active 
.v-enter-to 
.v-leave-from 
.v-leave-active 
.v-leave-to

然后把需要动画效果的组件放入transition标签中，vue便会自动调用这些样式类实现动画效果。
```
### 动画的使用
```
动画的实现基础就是需要你首先写好动画的样式类或者定义好动画效果，
而定义这些动画效果一般需要对css有深入的了解，
开发人员的时间会更多地向具体业务逻辑处理上倾斜，
所以一般就使用现成的动画类 animate.css 等，
有业务需求时再去查找具体如何使用。
```
### 退堂鼓
```
vue3的学习也应该先把握整体，
最后再针对局部去突破，
所以在vue动画这里我要合理合法的先舍弃了。
```
