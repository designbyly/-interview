## CSS部分

1. 两栏布局：垂直两栏，左边固定右边自适应。

   浮动

   flex

   position

   两端position

2. 三栏布局：垂直三栏，左右两栏宽度固定，中间自适应。

   左右分别设置绝对定位，中间设置外边距

   flex布局

   浮动布局，但是html中middle要放到最后

3. 圣杯布局和双飞翼布局：和三栏布局要求相同，不过中间列要写在前面保证优先渲染。

   圣杯布局：通过浮动和负边距实现

   双飞翼布局：多了一层

4. 实现一个三角形

   等边，等腰，等腰直角，普通

5. 正方形：使用CSS实现一个宽高自适应的正方形

   相对于屏幕宽度的比例设置

   内外边距的百分比相对于父元素的width来设置

   通过子元素的margin来设置

6. 扇形：实现一个1/4的圆，任意弧度的扇形

   通过border和border-radius

   类似三角形做法，加上父元素overflow：hidden

   通过子元素rotate%和父元素overflow：hidden

   通过skewY

   渐变设置

7. 水平垂直居中：实现子元素的水平垂直居中

   通过position和margin居中（需要知道juzi的长度）

   通过position和margin居中（2）

   flex居中

   position和transform居中

8. 清除浮动

   clear：both，BFC等

9. 弹出框效果

10. 导航栏

![image-20210426160227768](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210426160227768.png)

谢谢观看，橘子住院大家都会有一个好的前程！