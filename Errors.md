# 错误

> 用户输入错误

> 应用错误

> 不兼容状态错误

错误发生于一个应用不能完成所期待的事情，例如：
- 应用不能理解用户的输入
- 系统或者应用出错
- 一个用户试图同时运行不兼容的操作

设计应用使得用户能够轻松灵活地输入内容来最小化错误。应用应该接受通用数据格式，使用提示来提升用户理解。

如何强调错误：
- 明确沟通正在发生的事情
- 描述用户如何解决
- 保存尽可能多的用户输入内容


## 用户输入错误
一旦检测到用户输入错误，立马解决。如果检测到错误，取消表单的提交，如果是在提交之后监测到的，明确表达错误以及如何解决。

### 文本输入框
帮助文本可以出现在用户与表单上输入框交互之前、之时或者之后。

只在用户与一个输入框交互之后显示错误文本。如果用户输入不正确的数据，帮助文本可以转变为错误文本。

最小化表单文本到最必须的。并非每一个文本框都需要帮助文本和/或错误文本。

规范：

在文本框和下面的错误文本之间放置 16 dp 的垂直空间。

![](https://github.com/zhaochong/material-design/blob/master/images/12_1.png)
一个文本输入框的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_2.png)
一个带有错误提示的文本输入框的例子

### 白色背景的字体
- 错误: Roboto Regular 12sp #DD2C00
- 提示和帮助文本: #000000 with 38% opacity

![](https://github.com/zhaochong/material-design/blob/master/images/12_3.png)
白色主题用在这里显示以下情形：带有提示文本，带有错误文本，带有帮助文本，将错误文本作为帮助文本

### 黑色背景的字体
- 错误文本: Roboto Regular 12sp
- 提示和帮助文本: #FFFFFF with 30% opacity

![](https://github.com/zhaochong/material-design/blob/master/images/12_4.png)
黑色主题用在这里显示以下情形：带有提示文本，带有错误文本，带有帮助文本，将错误文本作为帮助文本

### 帮助和错误文本

![](https://github.com/zhaochong/material-design/blob/master/images/12_5.png)
带有帮助文本的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_6.png)
带有错误文本的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_7.png)
带有帮助文本的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_8.png)
带有错误文本的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_9.png)
带有帮助文本以及帮助文本和错误文本的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_10.png)
输入和错误文本

总共高：64 dp

输入文本上面的内边距：16 dp

输入文本下面的内边距：8 dp

错误文本上面和下面的内边距：4 dp

### 浮动文本标签相关错误
![](https://github.com/zhaochong/material-design/blob/master/images/12_11.png)
带有输入文本的浮动文本标签例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_12.png)
带有错误文本的浮动文本标签例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_13.png)
浮动文本标签的规格

![](https://github.com/zhaochong/material-design/blob/master/images/12_14.png)
总高：80 dp
标签文本上面的内边距：8 dp
输入文本上面和下面的内边距：8 dp
错误文本上面和下面的内边距：4 dp

### 文本输入框-上/下字符或者字数
一个字符计数器可以出现在用户与输入框交互之前、之时以及之后。直到用户接近字符限制时再考虑显示计数器。
- 计数器字体：Roboto Regular 12sp
- 计数器域有 16 dp 的额外底部内边距

### 带有字符计数器的单行
![](https://github.com/zhaochong/material-design/blob/master/images/12_15.png)
带有用户输入框的字符计数器单行的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_16.png)
带有错误文本的字符计数器单行的例子

### 带有字符计数器的多行文本
![](https://github.com/zhaochong/material-design/blob/master/images/12_17.png)
带有多行用户输入文本和字符计数器的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_18.png)
带有多行超出字数限制文本和字符计数器的例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_19.png)
这些情形的例子：带有用户输入文本的单行输入标签，带有错误文本的单行输入标签，带有用户输入文本的单行输入标签，带有错误文本的多行输入标签

![](https://github.com/zhaochong/material-design/blob/master/images/12_20.png)
文本输入框
单行输入标签的顶部内边距：16 dp
单行输入文本框的顶部和底部内边距：8 dp
完整输入区域的高度：88 dp

### 不相容的值
在一个用户与文本框交互之时和之后，为不相容的值显示错误。

如果两个或者多个输入框有不相容的输入：
- 在文本输入框中，表明需要解决。在下面添加一个错误消息。
- 在表单或者屏幕的顶部显示一个消息，总结需要解决的问题以及额外的解释。

### 提交表单时检测到的错误
重新加载带有合并错误内容的表单，在顶部进行滚动。单个输入框的错误消息可以在用户完成表单后解决。

![](https://github.com/zhaochong/material-design/blob/master/images/12_21.png)
表单例子

![](https://github.com/zhaochong/material-design/blob/master/images/12_22.png)
试图提交表单之后检测到错误的例子

### 不完整表单
对于留空的表单输入框，文本输入框和下面的错误消息应该都会有指示。

显示不完整表单错误来指示用户在完成表单之后跳过了一个输入框。如果不能在用户处理表单的时候检测到，在用户试图提交表单之后显示一个错误。

### 表单提交之前的多个错误
用户处理表单时的单个标签错误消息。

![](https://github.com/zhaochong/material-design/blob/master/images/12_23.png)
表单示例

![](https://github.com/zhaochong/material-design/blob/master/images/12_24.png)
不完整表单示例

### 单行错误列表
![](https://github.com/zhaochong/material-design/blob/master/images/12_25.png)
单行错误列表的例子


## 应用错误
应用错误独立于用户输入而发生

### 通常应用错误
一个错误发生时，一个应用应该显示加载提示直到错误消息显示。

不可用的功能可以被显示在 UI 中。并非每个错误都需要弹出一个新的组件。

如果可能的话，给你的用户一个动作来帮助他们关注到错误。

![](https://github.com/zhaochong/material-design/blob/master/images/12_26.png)
警告对话框：关于一个正在阻碍正常操作的错误的应用反馈

![](https://github.com/zhaochong/material-design/blob/master/images/12_26_2.png)
Snackbar：次要错误的应用反馈。Snackbar是短暂的，不要用它们来提示关键、持续以及大量的错误。


### 加载同步错误/失败
同步失败或者内容加载失败，用户应该可以与剩下的大部分应用内容进行交互。

![](https://github.com/zhaochong/material-design/blob/master/images/12_27.png)
屏幕/内容加载失败的空状态。

![](https://github.com/zhaochong/material-design/blob/master/images/12_28.png)
带有操作的容器/组件具体错误

### 连接
连接断掉时，用户应该能够和应用的其余大部分内容交互。

如果合适的话，显示一个连接来帮助用户完成他们的任务。只提供真正能有帮助的链接。例如，不要提供一个“再试一次”的选项，这种情况你是知道操作会失败的。

![](https://github.com/zhaochong/material-design/blob/master/images/12_29.png)
带有重试操作的 Snackbar

![](https://github.com/zhaochong/material-design/blob/master/images/12_30.png)
一个只有在线才能访问的页面的空状态


## 不兼容状态错误
不兼容状态错误发生于用户试图运行有冲突的操作，例如在飞行模式下打电话，或者访问一个没有权限账号的页面。通过清晰地沟通他们正在选择的状态以及剩余操作的完成，帮助用户预防这些情形的发生。当这些错误发生时，不要暗示这是用户的错。

### 通常不兼容性
澄清错误的原因

例如，在受限模式下，截屏和高级功能是不被允许的。

![](https://github.com/zhaochong/material-design/blob/master/images/12_31.png)
Snackbar 以及特别模式指示器

### 选择下线
当用户出于离线状态，但是试图做需要上线才能做的任务时，显示一个不显眼但是持续的指示器。

示例：
- 飞行模式下打电话
- 离线时的音乐可访问性

![](https://github.com/zhaochong/material-design/blob/master/images/12_32.png)
Snackbar

![](https://github.com/zhaochong/material-design/blob/master/images/12_33.png)
设备已经被放置到飞行模式的指示器

### 需要权限
如果你的应用在进行一个操作之前需要用户权限，在应用流程中包含权限请求，而不是把它当作一个错误。

如果应用的第一步就需要权限，考虑将它们包含到你应用的首轮实践中。

示例：
- 一个应用的权限已经发生变化。
- 应用内置的购买已经被禁用。

![](https://github.com/zhaochong/material-design/blob/master/images/12_34.png)
对话框
