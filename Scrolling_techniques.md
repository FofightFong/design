# 滚动技术

> 滚动

## 滚动
### 滚动区域
设计滚动行为时，应用条包含四个主要区域（称作`区块`），构成滚动结构：
- 状态条
- 工具条
- 标签条、搜索条
- 灵活区域：容纳一个预定比例的图片或者扩展应用条的空间

![](https://github.com/zhaochong/material-design/blob/master/images/16_1.png)
应用条组件可以包含：状态条、导航条、标签/搜索条，以及灵活区域

![](https://github.com/zhaochong/material-design/blob/master/images/16_2.png)
状态条、导航条、标签/搜索条以及灵活区域的例子

### 标准应用条
手机上标准应用条高度是 56 dp，更大一点的屏幕尺寸上是 64 dp。

有两种选项的滚动：
- 1.应用条可以将内容滚动到屏幕外面，当滚动返回时再次显示。
- 2.应用条可以固定在顶部，内容在下面进行滚动。

![](https://github.com/zhaochong/material-design/blob/master/images/16_3.png)
标准应用条

```
<video crossorigin="anonymous"  loop  controls width="360" height="640">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsR1lZQUxtWFRFMEU/patterns-scrolling-techniques_standard_appbar_xhdpi_004.webm" type="video/webm">
</video>
```
工具条在滚动时移出屏幕的动画效果

### 标签
[标准应用条](http://www.google.com/design/spec/layout/structure.html#structure-app-bar)是最重要的组件，包含下列区块：工具条、标签条或者灵活区域。

可以具有下列行为：
- 1.工具条滚动时，标签条固定在顶部。
- 2.应用条固定在顶部，内容在下面滚动。
- 3.工具条和标签条都随着内容滚动。反向滚动时标签条重现，反向滚动完成时工具条重现。

![](https://github.com/zhaochong/material-design/blob/master/images/16_4.png)
状态条、工具条以及标签条

```
<video crossorigin="anonymous"  loop  controls width="360" height="640">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsQ0ZQalNKOGxTNjA/patterns-scrolling-techniques_tabs_xhdpi_004.webm" type="video/webm">
</video>
```
工具条滚动、标签条以及应用条固定的动画效果。

### 灵活区域
应用条是灵活的，可以扩展来容纳更大的排版和图片。想要扩展应用条，添加一个灵活区域区块。

有两个显示选项：
- 1.可变区域收缩直到只剩工具条。导航条上的标题收缩到 20 sp。滚动到页面顶部时，可变区域以及标题再次回到位置。
- 2.整个应用条滚出屏幕。当用户反向滚动时，工具条变回到固定在顶部。当滚回所有内容时，可变区域和标题重新回到位置。

![](https://github.com/zhaochong/material-design/blob/master/images/16_5.png)
状态条、工具条以及可变区域

```
<video crossorigin="anonymous"  loop  controls width="360" height="640">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsRTM1M1lCWWZiN2c/patterns-scrolling-techniques-flexible_space_xhdpi_003.webm" type="video/webm">
</video>
```
显示滚动时灵活区域的动画

### 带有图片的灵活区域
使用可变区域在应用条中容纳想要的大小比例的图片。

本例中，视觉比例是4：3。滚动时，内容将图片推上去，收缩可变区域。转变的最后，图片以主色着色，不再受滚动影响。

![](https://github.com/zhaochong/material-design/blob/master/images/16_6.png)
状态条、工具条以及可变区域

```
<video crossorigin="anonymous"  loop  controls width="360" height="640">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQscXNQY3dNdVlYeTQ/patterns-scrolling-techniques_flex_space_image_xhdpi_003.webm" type="video/webm">
</video>
```
显示滚动时的可变区域和图片的动画效果

### 具有重叠内容的可变区域
内容可以重叠到应用条上

行为：
应用条的开始位置应该定位在内容的后面。对于向上滚动，应用条应该滚动的比内容快，直到内容与它不再重叠。一旦固定下来，应用条上升，让内容在下面滚动。

在这种交互中，应用条不能包含标签。

![](https://github.com/zhaochong/material-design/blob/master/images/16_7.png)
**可变区域**

状态条：24 dp

工具条：56 dp/64 dp

```
<video crossorigin="anonymous"  loop  controls width="360" height="640">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsRVpzZG0zZGVNSXM/patterns-scrolling-techniques_flex_space_overlap_xhdpi_003.webm" type="video/webm">
</video>
```
显示滚动时可变区域和重叠内容的动画效果

```
<video crossorigin="anonymous"  loop  controls width="360" height="115">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B3T7oTWa3HiFa3gtd2EzR2dsSDA/patterns_scrollingtechnique_flexibleoverlap.webm" type="video/webm">
</video>
```
z-轴图表，侧边视角
