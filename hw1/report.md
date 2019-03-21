# PAOGD_HW1 弹出的小球 实验报告

## 开发环境

 Blender2.8 beta

## 实验要求

+ 利用关键帧插值实现一个小球弹起动画，
+ 在动画过程中体现物体的旋转、平移、形变等
+ 利用shape key控制物体形变
+ 利用曲线编辑器graph editor调整物体在动画过程中的属性变化
+ 加分项：尝试给物体添加材质或纹理，使动画更加美观
+ 在满足要求的前提下可适当自由发挥

## 实现步骤

### 1. 物体创建和调整
shift+a 新建一个球体和一个平面，加上初始的立方体作为动画物体。使用快捷键g和s移动和缩放物体，调整物体位置和大小。shift/alt + 鼠标中键调整视角，滚轮缩放。

![][1]

### 2. 制作动画
1. 使用shape key制作立方体形变动画
首先点击立方体按TAB进入编辑模式，选中立方体的顶部的面并移动至底部

![][2]

按TAB推出编辑模式，创建两个shape key,选中key1，在下方值属性的数值轴中点击右键创建关键帧

![][3]

进入编辑模式，调整立方体的顶部的面并移动回顶部，将时间轴右键拖到想要的位置，将shape key窗口值属性的数值调至1并创建关键帧，完成形变动画

![][4]

2. 使用关键帧插值制作小球运动动画
调整小球位置以及时间轴位置，按i插入关键帧，blender会自动计算关键帧之间的运动

![][5]

3. 使用曲线编辑器graph editor实现小球弹跳效果
点击视图左边的按钮，进入曲线编辑器graph editor，TAB调出曲线设置窗口，设置小球下落的插值类型为反弹，可以较好的模拟出小球弹跳的状态。点击关键帧进行移动等操作调整出自己想要的效果

![][6]
![][7]

4. 使用shape key制作小球形变动画
与操作1类似，不过小球反弹形变后要恢复原状，即值属性再次设为0后创建关键帧

两种动画制作方式都可以用曲线编辑器graph editor进行调整

### 3. 光照，摄影与渲染
选中已有的光照物体，调整类型，光照强度，位置等属性。 调整摄影机的位置和角度。按z选择进入渲染模式可以看到光照的效果。

![][8]

### 4. 简单材质
材质的创建可以在右侧的material中添加设置，也可以打开shader editor来设置材质，后者的功能更强大。

![][9]
![][10]

## 实现场景

+ 镜头1：小球在盒子中

![][11]

+ 镜头2：盒子底部升起，小球被弹出

![][12]

+ 镜头3：小球掉落在地

![][13]

+ 镜头4：小球从地面反弹

![][14]

+ 镜头5：小球平稳落下

![][15]


## 实验总结
这次小球弹起实验让我初步了解blender，熟悉了blender的界面和基本操作，学会使用一些快捷键进行高效操作。除了使用关键帧制作动画这一主要内容，也简单了解了如何使用材质来丰富物体的形象。


  [1]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/1.png
  [2]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/2.1.1.png
  [3]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/2.1.2.png
  [4]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/2.1.3.png
  [5]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/2.2.png
  [6]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/2.3.1.png
  [7]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/2.3.2.png
  [8]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/3.png
  [9]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/4.1.png
  [10]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/4.2.png
  [11]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/scene1.png
  [12]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/scene2.png
  [13]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/scene3.png
  [14]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/scene4.png
  [15]: https://github.com/wei49/PAOGD_HW_Image/blob/master/hw1/scene5.png
  