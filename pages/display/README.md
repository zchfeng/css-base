# display属性
**作用**
 display属性规定了元素以何种方式展示，属性不支持继承
## 属性值
#### 1、默认值inline
此属性会显示为内联元素，元素是前后没换行符，设置margin，padding值无效
#### 2、none
此元素不会被显示.   
经常会考到，display:none与visibility: hidden有什么区别？    
都是看不见元素，但是display:none意思是不展示这个元素，该元素不占据空间，
而visibility: hidden只是将该元素隐藏了，只是用户不可见而已，占据页面空间
#### 3、block
此元素显示为块级元素，前后有换行符，可以设置宽 高 margin padding
#### 4、inline-block
行内块元素，结合了inline，block的特点，此元素有换行符，可以设置宽高
#### list-item
此元素作为列表显示，设置这元素可以将其当作ul标签使用
#### inherit
规定从父元素继承display属性的值
#### table
此元素作为块级元素显示（类似table）
#### .......