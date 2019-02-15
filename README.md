# scss
关于样式的记录
比起css，提供了变量，嵌套，混合，继承
# 变量 
通过$来声明一个变量，在真正的样式后面直接写$变量名。
# 嵌套
嵌套就是写成 父元素 子元素 {样式}，提高样式的可读性。
# 引入
----------不太懂
# 混合
----类似于一个方法，传递变量进入这个方法，然后调用这个方法，@mixin（写方法时） 和 @include（调用时）
# 继承
---比如说一个样式要在多个class里面的重复出现，就可以通过先声明 %变量名{}，然后再在class里面@extend %变量名。
# 引用父类选择器 &来代替父级

# absolute
相对于 static 定位以外的第一个父元素进行定位，元素的位置通过 "left", "top", "right" 以及 "bottom" 属性进行规定。
# fixed
生成绝对定位的元素，相对于浏览器窗口进行定位。元素的位置通过 "left", "top", "right" 以及 "bottom" 属性进行规定。
# relative
生成相对定位的元素，根据正常位置进行定位。
# static 
默认值。没有定位
# inherit
继承自父元素的position属性的值。
# transparent
   margin:38rpx 50rpx;
  border-top:33rpx solid transparent;
  border-left:54rpx solid #fff;
  border-bottom:33rpx solid transparent;
  拿这个举例，一个矩形就是从上到下，从下到上，距离会各有33rpx的透明平行透明空间，然后就是确定从左到右边的距离为54.
  # 正常图形的画法
  先是正常的class，如果是不规则的图形的话，写法是这样的，width：0；height：0；border-left：50px solid transparent;border-right: 50px solid transparent;border-bottom: 100px solid red;
  如果正常的情况下要在这个图像后续增加一个图像拼接，也就是伪类的方法。子元素的部分图像的画法可以借鉴上面那个部分的画法，除此之外，伪类如果需要对伪类图形进行定位的话position: absolute;top: 0px;left: 0px;同时正常的class也需要position: relative;的写法才能生效，以及伪类需要 content: "";里可以写字。
