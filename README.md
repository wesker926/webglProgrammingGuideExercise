# 这个仓库用于储存阅读[《webgl Programming Guide》](https://sites.google.com/site/webglbook/)时，所写的随章节练习项目。

#### 好记性不如烂笔头，敲一遍比什么都强。

### 练习于 2018.06.20

### [chapter02_01_HelloCanvas](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_01_HelloCanvas.html)
设置颜色缓冲区清除颜色，并清除画布。

### [chapter02_02_HelloPoint1](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_02_HelloPoint1.html)
绘制一个点，像素大小10.0，颜色红。

### 练习于 2018.06.21

### [chapter02_03_HelloPoint2](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_03_HelloPoint2.html)
和上个示例一样，不过使用了attribute标签将点的坐标从webgl系统外部赋予（自行修改了部分，生成100个点）。

### [chapter02_04_ClickedPoints](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_04_ClickedPoints.html)
设置交互内容，点击鼠标，在目标位置生成一个点。

### [chapter02_05_ColoredPoints](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_05_ColoredPoints.html)
在上一个示例的基础上，引入了uniform统一数据（这里也可以使用varying将数据从顶点着色器传入片元着色器，不过书里没这么用就算了），为点的颜色赋值（这里偷懒把颜色设置成了随机，没有根据象限赋值）。

### 练习于 2018.06.23

### [chapter03_01_MultiPoints](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_01_MultiPoints.html)
使用缓冲区对象，将多个点的坐标传入标签中，调用一次gl.drawArrays来绘制多个点。

由于webgl是标准归一化坐标到canvas的映射，所以这里全窗口化canvas会呈现屏幕比例的拉伸，由此例题开始修改canvas为正方形以适应示例。

### [chapter03_02_HelloTriangle](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_02_HelloTriangle.html)
通过三个点来绘制三角面（Face3 -> Triangle，三点确定一个平面）。

### [chapter03_03_HelloTriangle_LINES](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_03_HelloTriangle_LINES.html)
绘制线段，绘制方式为每两个点一条线段（v1 - v2 ; v3 - v4 ......），点为奇数个时忽略尾点。

### [chapter03_04_HelloTriangle_LINE_STRIP](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_04_HelloTriangle_LINE_STRIP.html)
绘制连续线段（v1 - v2 ; v2 - v3 ......）。

### [chapter03_05_HelloTriangle_LINE_LOOP](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_05_HelloTriangle_LINE_LOOP.html)
绘制连续的环线（首尾相连，v1 - v2 ; v2 - v3 ...... vn - v1）。

### [chapter03_06_HelloQuad](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_06_HelloQuad.html)
绘制正方形（两个三角面，带状排列，绘制方向为逆时针）。

### [chapter03_07_HelloQuad_FAN](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_07_HelloQuad_FAN.html)
绘制飘带（两个三角面，扇状排列）。

### [chapter03_08_TranslatedTriangle](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_08_TranslatedTriangle.html)
使用数学表达式来进行平移操作。

### [chapter03_09_RotatedTriangle](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_09_RotatedTriangle.html)
使用数学表达式来进行旋转操作。

### [chapter03_10_RotatedTriangle_Matrix](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_10_RotatedTriangle_Matrix.html)
使用4*4变换矩阵来进行旋转操作。

### [chapter03_11_TranslatedTriangle_Matrix](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_11_TranslatedTriangle_Matrix.html)
使用4*4变换矩阵来进行平移操作。

### [chapter03_12_ScaledTriangle_Matrix](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_12_ScaledTriangle_Matrix.html)
使用4*4变换矩阵来进行缩放操作。

### 练习于 2018.06.24

### [chapter04_01_RotatedTriangle_Matrix4](http://www.wesker926.com/webglProgrammingGuideExercise/chapter04_01_RotatedTriangle_Matrix4.html)
将上一章节的示例中，对变换矩阵的手动创建变为本书所提供的矩阵函数库，方便使用。

### [chapter04_02_RotatedTranslatedTriangle_Matrix4](http://www.wesker926.com/webglProgrammingGuideExercise/chapter04_02_RotatedTranslatedTriangle_Matrix4.html)
进行复合矩阵的练习，先平移，后旋转。

因为该矩阵库中，复合矩阵（矩阵乘法）进行复合时是右乘，复合矩阵对原始坐标是左乘，所以代码中是先设置旋转，后追加平移。

(<旋转矩阵> X <平移矩阵>) X <原始坐标>  --  矩阵乘法满足结合律，不满足交换律，顺序很重要，详见线性代数教材。

### [chapter04_03_TranslatedRotatedTriangle_Matrix4](http://www.wesker926.com/webglProgrammingGuideExercise/chapter04_03_TranslatedRotatedTriangle_Matrix4.html)
上一示例的反向操作，先旋转，后平移。

### [chapter04_04_RotatingTriangle](http://www.wesker926.com/webglProgrammingGuideExercise/chapter04_04_RotatingTriangle.html)
简单动画，旋转的三角形。

由于已有一定的web动画基础，由此例开始，将使用自己熟悉的代码风格和结构。并为以后所有动画类示例追加stats.js状态监控。

本示例中，作者使用了requestAnimationFrame来更新动画，使用了elapsedTime/deltaTime等类似的结构来计算更新值。

由于当页面离屏时，浏览器渲染停止，但计时未停止（Date.now()），所以会导致delta的累积，我在这里使用了一个监听函数消除累积（表现为当切出页面再回来，图形保持在离开时的状态，即离开的这段deltaTime清零）。

### [chapter04_05_RotatingTranslatedTriangle](http://www.wesker926.com/webglProgrammingGuideExercise/chapter04_05_RotatingTranslatedTriangle.html)
简单动画，边旋转边平移的物体。

### [chapter04_06_RotatingTranslatedTriangle_withButtons](http://www.wesker926.com/webglProgrammingGuideExercise/chapter04_06_RotatingTranslatedTriangle_withButtons.html)
简单动画，边旋转边平移的物体，附加变速按钮以修改平移速度。

### 练习于 2018.06.25 - 2018.06.26

### [chapter05_01_MultiAttributeSize](http://www.wesker926.com/webglProgrammingGuideExercise/chapter05_01_MultiAttributeSize.html)
通过多个缓冲区的方式传入除坐标外顶点的其他信息（顶点尺寸）。

### [chapter05_02_MultiAttributeSize_Interleaved](http://www.wesker926.com/webglProgrammingGuideExercise/chapter05_02_MultiAttributeSize_Interleaved.html)
通过单个缓冲区交错组织的方式传入除坐标外顶点的其他信息（顶点尺寸）。

### [chapter05_03_MultiAttributeColor](http://www.wesker926.com/webglProgrammingGuideExercise/chapter05_03_MultiAttributeColor.html)
通过单个缓冲区交错组织的方式传入除坐标外顶点的其他信息（顶点尺寸，颜色），然后通过varying变量将颜色信息从顶点着色器传递到片元着色器。

### [chapter05_04_ColoredTriangle](http://www.wesker926.com/webglProgrammingGuideExercise/chapter05_04_ColoredTriangle.html)
将绘制方式由点变为三角面，理解通过光栅化将图元（矢量信息）转换为片元（像素）的过程，类似于ps中的矢量图形栅格化。

### [chapter05_05_TexturedQuad](http://www.wesker926.com/webglProgrammingGuideExercise/chapter05_05_TexturedQuad.html)
为二维平面加载纹理（纹理图片），特别注意的是图片的尺寸如果不是2的次幂，需要将水平和垂直填充方式设置为gl.CLAMP_TO_EDGE（使用边缘值）。

### [chapter05_06_TexturedQuad_Repeat](http://www.wesker926.com/webglProgrammingGuideExercise/chapter05_06_TexturedQuad_Repeat.html)
理解重复填充方式。

### [chapter05_07_TexturedQuad_Repeat_Mirror](http://www.wesker926.com/webglProgrammingGuideExercise/chapter05_07_TexturedQuad_Repeat_Mirror.html)
理解镜像重复填充方式。

### [chapter05_08_MultiTexture](http://www.wesker926.com/webglProgrammingGuideExercise/chapter05_08_MultiTexture.html)
双纹理叠加（矢量相乘方法）。