# 加载图片

> 加载图片

## 加载图片
插图和照片可以在排列时以三种相位进行加载和转换，而不仅仅依赖于透明度转换。结合透明度、曝光度以及饱和度变化来满足你的需求。

曝光度为低对比度以及低饱和度进行调整。一旦透明度达到 100%，会达到全色饱和度。

低对比效果结合 gamma 和 black output（专为黑色图片）的转换。

![](https://github.com/zhaochong/material-design/blob/master/images/14_1.png)
**加载图片时的透明度、曝光度以及饱和度建议**

透明度：0% 开始，100%结束

曝光度：Gamma，Black output（专为黑色图片）

饱和度: 0 或者 20% 开始, 100% 结束

![](https://github.com/zhaochong/material-design/blob/master/images/14_2.png)
低透明度以及低对比度

![](https://github.com/zhaochong/material-design/blob/master/images/14_3.png)
完全透明和曝光

![](https://github.com/zhaochong/material-design/blob/master/images/14_4.png)
颜色饱和度

### 逐渐增强过程
目睹图片逐渐增强，就像照片的冲洗过程一样。

注意不要让图片过度曝光。

![](https://github.com/zhaochong/material-design/blob/master/images/14_5.png)
正确

![](https://github.com/zhaochong/material-design/blob/master/images/14_6.png)
错误

### 持续时间
加载图片时推荐长一点的持续时间，过渡时推荐短一点的持续时间。

```
<video crossorigin="anonymous"  loop  controls width="360" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B08MbvYZK1iNM2xXbGwyN2pISUE/patterns-imagerytreatment-imageload-transition_large_xhdpi.webm" type="video/webm">
</video>
```
加载和过渡动画

### 大一点的屏幕
这个过程对于大一点的屏幕比较理想，例如加载 Chrome OS 的墙纸。

```
<video crossorigin="anonymous"  loop  controls width="760" height="504">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B3T7oTWa3HiFWUZZN05CQ2Vva0k/patterns_loadingimages_largescreen.webm" type="video/webm">
</video>
```
动画显示了在大一点的屏幕上加载 Chrome OS 墙纸。

### 添加动画
给正在加载的图片一个小的位移。这里账户切换中的背景图片水平移动。

```
<video crossorigin="anonymous"  loop  controls width="360" height="360">
<source src="http://materialdesign.qiniudn.com/publish/material_v_4/material_ext_publish/0B0NGgBg38lWWdlUtbnpFOUMzRUk/patterns-loadingimages-loading-070901_Load_Add_Animation_xhdpi_002.webm" type="video/webm">
</video>
```
显示添加移动的视频。
