
# 环境

> 内容
> 三维世界（3D world）	
> 光影关系（Light and shadow）

三维世界（3D world）
Material 环境是一个三维的空间，这意味着每个对象都有 x ， y ， z 三维坐标属性，z轴垂直于显示平面，并延伸向用户视角,每个 material 元素在z轴上占据一定的位置并且有一个 1dp 厚度的标准。
在网页上，z 轴被用来分层而不是为了视角。3D 空间通过操纵 y 轴进行仿真。

! https://github.com/zhaochong/material-design/blob/master/images/1.png
具备 x，y 和 z 轴的 3D 空间
[1]:https:://github.com/younghz/Markdown

光影关系（Light and shadow）
在 material 环境中，虚拟的光线照射使场景中的对象投射出阴影，主光源投射出一个定向的阴影，而环境光从各个角度投射出连贯又柔和的阴影。
material环境中的所有阴影都是由这两种光投射产生的，阴影是光线照射不到的地方,因为各个元素在z轴上占据了不同大小的位置遮挡住了这些光线。








