# Material 语言属性

Material 拥有一些确定不变的典型固有性质。理解这些性质会在某种程度上帮助你遵循 Material 的设计愿景来利用它。

> 物理属性

> Material 变化

> material 活动

## 物理属性
Material 在 x 和 y 维度上长度不同（用 dp 计），厚度不变（1 dp）。

![正确：Material 的高度和宽度都可以变化。](https://github.com/zhaochong/material-design/blob/master/images/2.png)  
正确：Material 的高度和宽度都可以变化。

![错误：Material 总是 1 dp 厚。](https://github.com/zhaochong/material-design/blob/master/images/3.png)  
错误：Material 总是 1 dp 厚。

Material 会产生阴影。
阴影效果自然来自于material 元素的相对高度（z 坐标）。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsM01aOVkzWXFYb1k/inline%20whatismaterial-materialprop-physicalprop-PaperShadow_01_xhdpi_008.webm" type="video/webm">
</video>
```
正确：阴影描绘 material 元素间的相对高度。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsRGhTci1mN2dWUW8/inline%20whatismaterial-materialprop-physicalprop-PaperShadow_02_xhdpi_008.webm" type="video/webm">
</video>
```
错误：阴影和着色的 material 从不相似。

不管任何形状和颜色，内容都显示在 material 上。内容不会增加 material 的厚度。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsaGVXTFRCVG1iU2M/whatismaterial-materialprop-physicalprop-InkDisplay_xhdpi_006.webm" type="video/webm">
</video>
```
正确说法：Material 可以表现任何形状和颜色。


内容可以独立于 material 表现出来，但是会被 material 的边界限制。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsdnpyMjVKeFNvVm8/whatismaterial-materialprop-physicalprop-InkBehavior_xhdpi_006.webm" type="video/webm">
</video>
```
正确说法：内容行为可以独立于 material 行为。

Material 是固体的。
输入事件不能通过 material。

![正确说法：输入事件只影响 material 的前景。](https://github.com/zhaochong/material-design/blob/master/images/4.png)  
正确说法：输入事件只影响 material 的前景。

![错误说法：输入事件不能通过 material。](https://github.com/zhaochong/material-design/blob/master/images/5.png)  
错误说法：输入事件不能通过 material。

多个 material 元素不能同时占据空间中的同一个点。

![正确说法：利用高度来区分material元素，是防止多个 material 元素同时占据空间中同一个点的一种方法。](https://github.com/zhaochong/material-design/blob/master/images/6.png)  
正确：利用高度来区分 material 元素，是防止多个 material 元素同时占据空间中同一个点的一种方法。

![错误说法：多个material元素不能同时占据空间中的同一个点。](https://github.com/zhaochong/material-design/blob/master/images/7.png)  
错误：多个 material 元素不能同时占据空间中的同一个点。

Material 不能穿过其他 material。

比如：当改变高度时，一张 material 不能穿过另一张 material。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsekRnTGVlVEQzNXc/whatismaterial_properties_physical_07_xhdpi_009.webm" type="video/webm">
</video>
```
错误。Material 不能穿过另一种 material。


## Material 变化
Material 可以改变形状。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsRjREbXNsZXBrTFU/whatismaterial-materialprop-transformingmaterial-PaperShape_xhdpi_005.webm" type="video/webm">
</video>
```
Material 可以改变形状。

Material 只能沿着它的平面伸展和收缩。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsRjREbXNsZXBrTFU/whatismaterial-materialprop-transformingmaterial-PaperShape_xhdpi_005.webm" type="video/webm">
</video>
```
正确。Material 只能沿着它的平面伸展和收缩。

Material从不弯曲或者折叠。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsMXhFNUo2WmJrLWc/whatismaterial-materialprop-transformingmaterial-PaperBendFold_xhdpi_006.webm" type="video/webm">
</video>
```
不正确。Material 从不弯曲或者折叠。

很多张的 material 拼接在一起可以变成单张的 material。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsRmdDaEl6aTVGREU/whatismaterial-materialprop-transformingmaterial-PaperHeal_xhdpi_004.webmm" type="video/webm">
</video>
```
很多张的 material 拼接在一起可以变成单张的 material。

当拆分以后，material 可以恢复正常。比如，你从一张 material 里移除一部分以后，这张 material 又会变成一整张。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsQV9PS2Q0anFoZzg/whatismaterial-materialprop-transformingmaterial-PaperSplitHeal_xhdpi_005.webm" type="video/webm">
</video>
```
Material 可以拆分开，然后又变得完整。


## material 活动
在环境中的任何地方，material 都可以自然的生成或破坏。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQseERpUzUxRVRtMGs/whatismaterial-materialprop-movementmaterial-PaperPointExpand_xhdpi_005.webm" type="video/webm">
</video>
```
Material 可以自然地生成或破坏。

Material 可以沿任意轴移动。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsWkhGeVpPNVdZbE0/whatismaterial-materialprop-movementmaterial-PaperMove_xhdpi_008.webm" type="video/webm">
</video>
```
Material 可以沿各种轴移动。

沿Z轴运动通常是用户与 material 相互作用的结果。

```
<video crossorigin="anonymous"  loop  controls width="760" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsYWJoQjFCYmdvU3c/whatismaterial-materialprop-movementmaterial-Material_Response_xhdpi_003.webm" type="video/webm">
</video>
```
沿Z轴运动是由于用户的相互影响造成的。









