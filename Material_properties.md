# Material 语言属性

Material 拥有一些确定不变的典型固有性质。理解这些性质会在某种程度上帮助你遵循 Material 的设计愿景来利用它。

> 物理属性

> Material变化

> material活动

## 物理属性
Material 在 x 和 y 维度上长度不同（用 dp 计），厚度不变（1 dp）。

![正确：Material 的高度和宽度都可以变化。](https://github.com/zhaochong/material-design/blob/master/images/2.png)
正确：Material 的高度和宽度都可以变化。

![错误：Material 总是 1 dp 厚。](https://github.com/zhaochong/material-design/blob/master/images/3.png)
错误：Material 总是 1 dp 厚。

Material 会产生阴影。
阴影效果自然来自于material 元素的相对高度（z 坐标）。

正确：阴影描绘 material 元素间的相对高度。
错误：阴影和着色的 material 从不相似。

不管任何形状和颜色，内容都显示在 material 上。内容不会增加 material 的厚度。
正确说法：Material 可以表现任何形状和颜色。


内容可以独立于material表现出来，但是会被material的边界限制。
正确说法：内容行为可以独立于material行为。

Material是固体的。
输入事件不能通过material。

![正确说法：输入事件只影响 material 的前景。](https://github.com/zhaochong/material-design/blob/master/images/4.png)
正确说法：输入事件只影响 material 的前景。
![错误说法：输入事件不能通过 material。](https://github.com/zhaochong/material-design/blob/master/images/5.png)
错误说法：输入事件不能通过 material。

多个material元素不能同时占据空间中的同一个点。

![正确说法：利用高度来区分material元素，是防止多个 material 元素同时占据空间中同一个点的一种方法。](https://github.com/zhaochong/material-design/blob/master/images/6.png)
正确说法：利用高度来区分 material 元素，是防止多个 material 元素同时占据空间中同一个点的一种方法。
![错误说法：多个material元素不能同时占据空间中的同一个点。](https://github.com/zhaochong/material-design/blob/master/images/7.png)
错误说法：多个material元素不能同时占据空间中的同一个点。

Material不能穿过其他material。
比如：当改变高度时，一张material不能穿过另一张material。


错误说法：Material不能穿过另一种material。


## Material 变化
Material可以改变形状。

Material可以改变形状。

Material只能沿着它的平面伸展和收缩。

Material从不弯曲或者折叠。
Material从不弯曲或者折叠。

很多张的material拼接在一起可以变成单张的material。
![很多张的material拼接在一起可以变成单张的material。](https://material-design.storage.googleapis.com/publish/material_v_4/material_ext_publish/0B6Okdz75tqQsRmdDaEl6aTVGREU/whatismaterial-materialprop-transformingmaterial-PaperHeal_xhdpi_004.webm)
很多张的material拼接在一起可以变成单张的material。

当拆分以后，material可以恢复正常。比如，你从一张material里移除一部分以后，这张material又会变成一整张。
Material可以拆分开，然后又变得完整。


## material 活动
在环境中的任何地方，material都可以自然的生成或破坏。

Material可以自然地生成或破坏。


Material可以沿任意轴移动。

Material 可以沿各种轴移动。


沿Z轴运动通常是用户与material相互作用的结果。

沿Z轴运动是由于用户的相互影响造成的。









