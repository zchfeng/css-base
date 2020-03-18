# css重点知识点总结
## display： 属性规定元素应该生成的框的类型
### none  元素不显示
### block 块级元素
### inline 默认  行业元素
### inline-block 行块级元素
### list-item  列表显示
### table 块级表格显示
### inherit 继承父级display属性

## position：定位属性
### absolute  绝对定位，相对于static定位以外的第一个父元素定位
### relative  相对定位，相对其正常位置定位
### fixed 绝对定位，相对浏览器窗口定位
### static 默认值，在正常的流中
### inherit 从父级继承属性

## flex 弹性布局  https://www.cnblogs.com/lytwajue/p/7293918.html
### display: flex 声明弹性盒模型
### flex-direction  决定主轴方向  属性：row、row-reverse、colum、column-reverse
### flex-warp  是否换行   属性： nowrap、wrap、wrap-reverse
### flex-flow  flex-direction和flex-warp的简写形式
### justify-content 主轴对齐方式  属性：flex-start、flex-end、center、space-between、space-around
### align-items 属性定义每项侧轴对齐方式  属性：flex-start、flex-end 、 center 、 baseline、stretch
### align-content 容器在侧轴方向上有额外空间，怎么每排布一行，当容器只有一行，不起作用。 属性：flex-start、 flex-end、 center 、space-between 、 space-around、stretch

### order 项目排列顺序，值越小排的越靠前，默认0
### flex 
### flex-grow属性定义项目的放大比例，默觉得0，即假设存在剩余空间也不放大。
### flex-shrink属性定义了项目的缩小比例，默觉得1。即假设空间不足该项目将缩小。
### flex-basis属性定义了在分配多余空间之前，项目占领的主轴空间（main-size）。
### align-self属性同意单个项目有与其它项目不一样的側轴对齐方式，可覆盖align-items属性。