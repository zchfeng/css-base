# flex（弹性盒布局Flexbox）display:flex
#### 基本概念
采用 Flex 布局的元素，称为 Flex 容器（flex container），简称"容器"。它的所有子元素自动成为容器成员，称为 Flex 项目（flex item），简称"项目"。    
三个核心概念    
    -flex项（子元素），需要布局的元素   
    -flex容器（父元素），其包含flex项   
    -排列方向，这决定了flex项的布局方向
#### 容器属性
###### 1、flex-direction: 主轴方向
 row(默认值)：主轴为水平方向，起点为左端   
 row-reverse: 主轴为水平方向，起点为右端   
 column: 主轴为垂直方向，起点为上沿    
 column-reverse: 主轴为垂直方向,起点在下沿 
###### 2、flex-warp:换行
nowrap（默认）: 不换行  
warp: 换行，第一行在上方   
warp-reverse: 换行，第一行在下方
###### 3、justify-content: 主轴对齐方式
flex-start(默认值)： 左对齐 
flex-end : 右对齐   
center： 居中   
spance-between: 两端对齐，项目之间的间隔相等    
span-around: 每项两侧的间隔相等，所以项目之间的间隔也边框的间隔大一倍  
###### 4、align-items: 交叉轴对齐方式(只有一排项）
flex-start: 交叉轴起点对齐  
flex-end: 交叉轴终点对齐    
center: 交叉轴的中点对齐    
baseline: 项目的第一行文字的基线对齐    
stretch(默认值): 如果项目未设置高度或设为auto ,将占整个容器的高度
###### 5、align-content： 交叉轴对齐方式（有多排项）
flex-start: 与交叉轴的起点对齐  
flex-end: 与交叉轴的终点对齐    
center: 与交叉轴的中点对齐  
space-between: 与交叉轴两端对齐，轴线之间的间距平均分布     
space-around: 每根轴线两侧的间隔相等，所以，轴线之间的间隔比轴线与边框的间隔大一倍    
stretch(默认值)： 轴线占满整个交叉轴    

#### 项目属性
1、order：数字值，项目的排列顺序，数值越小，排列越靠前  
2、flex-grow: 项目放大的比例，默认为0，不会放大  
3、flex-shrink: 项目的缩小比例，默认为1，空间不足时该项目会缩小  
4、flex-basis    
5、flex:属性flex-grow、flex-shink、flex-basis的简写，默认为0 1 auto 
6、align-self：属性允许单个项目与其他项目不一样的对齐方式，可覆盖align-items



[参考文档](https://www.cnblogs.com/hellocd/p/10443237.html)