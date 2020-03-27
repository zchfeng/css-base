# 2D、3D及动画
### 1、2D和3D（transform）
#### 属性：
1. 位移：translate(x,y)  
   x表示水平移动方向，y垂直方向的距离，需要带单位px,可以取负值   
   translateX(x): 指定方向设置位移，沿X轴移动   
   translateY(Y): 指定方向设置位移，沿Y轴移动          
   translateZ(z): 指定方向设置位移，沿Z轴移动（需要声明3D属性）   
   属性值也可以取%，百分比大小的参照物是元素的宽高  
   说明：translate（）位移的效果和定位里的relative的效果是类似的，都是在当前位置进行位移的，对其元素的布局是没有影响的，原来的位置的保留的。
    
    
2. 缩放scale(x,y)    
    说明： 属性值代表的是倍数，是不用加单位； 0——1 之间是 缩小的效果， 大于1的时候都是放大效果；当设置一个值时代表水平和垂直都放大或者缩小     
   scaleX(): 水平方向的缩放比例    
   scaleY(): 垂直方向的缩放比例  
   scaleZ(): Z轴方向的缩放比例（需要声明3D属性）  
    
    
3. 旋转rotat()  
   说明: 属性值的单位是度（deg）,只能放一个属性值 ，正值：顺时针旋转； 负值： 逆时针旋转；
   rotate(): 沿中心点旋转
   roateX(): 沿X轴旋转  
   roateY(): 沿Y轴旋转  
   roateZ(): 沿Z轴旋转（需要声明3D属性）

4. 倾斜skew()   
   说明：属性值的单位是度（deg） ；属性值为正值：向左 或向上倾斜 负值：向右或向下倾斜,元素通过 transform进行变形时，都是对其他元素的布局不产生影响的。不脱离文档流。变形时元素默认情况下都是沿着元素的中心点去变形的   
    skew()  一个值的时候 代表 沿X轴倾斜, 值1： 沿X轴的倾斜,值2：沿Y轴的倾斜    
    skewX（） 沿X轴的倾斜
    skewY（） 沿Y轴的倾斜

5. 原点设置属性：transform-origin   
    定义：transform-origin是变形原点，也就是该元素围绕着那个点变形或旋转，该属性只有在设置了transform属性的时候起作用；
    说明：transform-origin：值1 值2 ； 值1： 水平 值2： 垂直
    px % left top right bottom ;

6. backface-visibility ：隐藏被旋转的 div 元素的背面    
    backface-visibility:visible;可见 （默认值）     
backface-visibility:hidden;不可见   
backface-visibility的bug:如果元素翻转后结束后显示在上一层，给他加一个背景色就可以解决了。
**注：当使用复合式写法的时候，他们顺讯不同，会导致结果不一样，他们执行的顺讯是从后向前解析的。**  

#### 2.perspective:视角距离（x px）
#### 3.perspective-origin:视角位置(默认perspectice-origin: 50% 50%,第一个数值是 3D 元素所基于的 X 轴，第二个定义在 y 轴上的位置)

#### 4.transform-style:视角类型，默认是flat，如果你要在元素上视线3D效果的话，就必须用上transform-style: preserve-3d

### 5.Animation 动画组成
```
    .list div:first-child {
     animation: dropdown 8s linear infinite;
    }
    @keyframes dropdown {
        0% { margin-top: 0px;}
       /** 暂停效果 */
       10% { margin-top: 0px;}
       50% { margin-top: -100px;}
       60% { margin-top: -100px;}
       90% { margin-top: -200px;}
      100% { margin-top: -200px;}
    }
```
[来源](https://www.sohu.com/a/167061536_610671)