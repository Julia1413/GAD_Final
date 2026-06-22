# 期末作业说明

23121413 沈怡均

UE项目文件Github链接：[GAD_UE_Shenyijun](https://github.com/Julia1413/GAD_Final/tree/master/GAD_UE_Shenyijun)

Wwise项目文件Github链接：[GAD_Wwise_Shenyijun](https://github.com/Julia1413/GAD_Final/tree/master/GAD_Wwise_Shenyijun)

视频、图片、说明文档pdf链接：[GAD_Wwise_Shenyijun](https://github.com/Julia1413/GAD_Final/tree/master/GAD_Wwise_Shenyijun)

网盘链接（以防万一）：[23121413\_沈怡均\_游戏音频设计期末作业](https://pan.baidu.com/s/1476yDonPeppfqlvfbgTGmQ?pwd=3uu4) 提取码: 3uu4



作业演示视频：[演示视频](https://pan.baidu.com/s/1VMTIMItw3gnrvxACGkZk7g?pwd=a1tv)

## 一、作品概述

本次作业主要实现了以下几点：

1. 空间音频

   * Effect 插件和相应的 3D 化 Positioning 设置，以及声音传送到 Aux Bus 的设置
   * 在地图场景中使用 Room 和 Portal 对象创建室内外空间和联通，以及组件内各个 Component 相对应功能的具体设置
   * 室外空间播放环境声基底，以及实现室内外空间联通处的衰减过渡效果
   * 室内空间设置混响效果
2. 基础环境声

   * 3D 化 Positioning 设置和 Attenuation 衰减曲线
3. 篝火物件

   * Random播放设置和Blender声音整合
   * 使用蓝图对象的方式创建一个篝火物件，摆放至地图中的室内空间，正确播放且带有混响效果
4. Female\_Voice

   * Sequence播放设置
   * 使用蓝图对象的方式创建一个Voice物件，摆放至地图中的室内空间，正确播放且带有混响效果
   * 声音穿透墙壁效果
5. 角色脚步

   * Game Sync Switch 2种鞋子类型和7种材质类型和相应的 Switch Container 嵌套层级结构的具体设置
   * 角色跑步声资产以 Notify 的形式配置在角色动画中，并指定到对应的 Socket 上
   * 创建7种 Material 材质 Dirt、Rock、Wood 、 Grass、DeepWater、MiddleWater和ShallowWater，以及对应的 Physical Material 和 Surface Type，并将材质正确配置到场景中
   * 对 Notify 的功能进行改造，实现 Raycast 射线检测材质的功能

项目地图：[Map](https://github.com/Julia1413/GAD_Final/blob/main/1.png)

## 二、空间音频

* Effect 插件和相应的 3D 化 Positioning 设置，以及声音传送到 Aux Bus 的设置 [Wwise室内混响效果](https://github.com/Julia1413/GAD_Final/blob/main/2.png)
* 在地图场景中使用 Room 和 Portal 对象创建室内外空间和联通，以及组件内各个 Component 相对应功能的具体设置 [UE中的Room对象](https://github.com/Julia1413/GAD_Final/blob/main/3.png)
* 室外空间播放环境声基底，以及实现室内外空间联通处的衰减过渡效果 [UE中的Portal对象](https://github.com/Julia1413/GAD_Final/blob/main/4.png)
* 室内空间设置混响效果 [室内空间设置混响效果](https://github.com/Julia1413/GAD_Final/blob/main/5.png)

## 三、基础环境声

* 3D 化 Positioning 设置和 Attenuation 衰减曲线 [环境声3D 化 Positioning 设置和 Attenuation 衰减曲线](https://github.com/Julia1413/GAD_Final/blob/main/6.png)

## 四、篝火物件

* Sequence播放设置
* 使用蓝图对象的方式创建一个Voice物件，摆放至地图中的室内空间，正确播放且带有混响效果[篝火物件的Random播放设置和Blender声音整合、混响效果](https://github.com/Julia1413/GAD_Final/blob/main/7.png)
* 声音穿透墙壁效果[UE中篝火蓝图](https://github.com/Julia1413/GAD_Final/blob/main/8.png)

## 五、Female\_Voice

* Sequence播放设置[Female\_Voice的Sequence播放设置、混响效果、声音穿透效果](https://github.com/Julia1413/GAD_Final/blob/main/9.png)
* 使用蓝图对象的方式创建一个Voice物件，摆放至地图中的室内空间，正确播放且带有混响效果[UE中Female\_Voice蓝图](https://github.com/Julia1413/GAD_Final/blob/main/10.png)
* 声音穿透墙壁效果

## 六、角色脚步

* Game Sync Switch 2种鞋子类型和7种材质类型和相应的 Switch Container 嵌套层级结构的具体设置[室内空间设置混响效果](https://github.com/Julia1413/GAD_Final/blob/main/11.png)
* 角色跑步声资产以 Notify 的形式配置在角色动画中，并指定到对应的 Socket 上[UE角色动画序列](https://github.com/Julia1413/GAD_Final/blob/main/12.png)
* 创建7种 Material 材质 Dirt、Rock、Wood 、 Grass、DeepWater、MiddleWater和ShallowWater，以及对应的 Physical Material 和 Surface Type，并将材质正确配置到场景中[UE角色AkEvent蓝图（局部）](https://github.com/Julia1413/GAD_Final/blob/main/13.png)
* 对 Notify 的功能进行改造，实现 Raycast 射线检测材质的功能[UE角色AkEvent蓝图](https://github.com/Julia1413/GAD_Final/blob/main/14.png)

## 七、遇到的困难

1.漏看一集教程，导致项目衔接不上，耽误了很多时间，希望老师能给教程按照观看顺序编号
2.在制作Female Voice的声音穿透效果的时候，总是无法实现声音穿透墙壁的效果，后来通过Positioning设置了Diffraction and Transmission，并调整了Transmission曲线，实现了穿透效果
3.在制作不同水深的脚步声时，一开始我没有把这三种类型作为HighHeel的子项，而是作为另一种鞋型，但是并不能在Ue里正常播放。于是我把这三种类型作为HighHeel中Material的子项，依照教程实现了这种效果。

## 八、小结

项目制作过程总体来说非常顺利，教程非常详细全面，结构清晰逻辑严密。听了这门课后我对UE和Wwise的了解更进了一步，非常有利于我进行自己的游戏设计。更重要的是，这门课让我认识到声音在游戏中的作用非常关键。在之后的学习和生活中，我会有意识的关注游戏中的音频设计，并从中学习。
