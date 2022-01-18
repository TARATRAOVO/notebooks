## 导入模型与动画
### 模型文件三部分？
materials
model（avatar在里面）
textures
### 模型紫红色？
材质丢失或者渲染故障
### 出现材质丢失或者故障的原因与解决？
传统3D模版与URP不兼容。
使用unity自动升级材质完成：
edit-render pipeline-universal render pipeline-upgrade

### game窗口放置推荐？
右下
display最好fress aspect
### 模型包含什么？
model
rig
animation
materials
### 模型如何使用外部的人类动画？
首先装好骨骼系统。
Animation type 选择人形的（humanoid）
avatar（骨骼） defination 如果模型自带动作，就 create from this model
应用上，骨骼系统整理好了。
可以点configure 检查。
实心的⭕️，指代必须拥有的关节，虚线的指代可有可无。
接着配置上动画。（使用RM动画好）
点模型组合文件，看到animator，发现控制器没对应。
在文件中装创建一个控制器 create-animator controller
打开动画控制器窗口，window-animation-animator
选中我们的文件模型组合文件之后，控制器窗口就显示的是我们对应模型的控制窗口了。
然后选文件，拖到控制窗口里面，就加好动作了！

### 如何在设置transition条件（动画变化条件）？

触发transition的变量时在animator窗口中，然后使用脚本来控制这个变量.
直接创建一

### RM动画有什么特别的？
动画动的时候，角色的位置真的会移动。

### 如何读取键盘？

if(Input.GetKey("keyname"))

### 

### 动作文件是怎么样的？
三条线加三角形图标的。

