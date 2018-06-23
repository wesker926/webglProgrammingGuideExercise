# 这个仓库用于储存阅读[《webgl Programming Guide》](https://sites.google.com/site/webglbook/)时，所写的随章节练习项目。

#### 好记性不如烂笔头，敲一遍比什么都强。

### 练习于 2018.06.20

### [chapter02_01_HelloCanvas](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_01_HelloCanvas.html)
设置颜色缓冲区清除颜色，并清除画布。

### [chapter02_02_HelloPoint1](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_02_HelloPoint1.html)
绘制一个点，像素大小10.0，颜色红。

### 练习于 2018.06.21

### [chapter02_03_HelloPoint2](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_03_HelloPoint2.html)
和上个示例一样，不过使用了attribute标签将点的坐标从webgl系统外部赋予。（自行修改了部分，生成100个点）

### [chapter02_04_ClickedPoints](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_04_ClickedPoints.html)
设置交互内容，点击鼠标，在目标位置生成一个点。

### [chapter02_05_ColoredPoints](http://www.wesker926.com/webglProgrammingGuideExercise/chapter02_05_ColoredPoints.html)
在上一个示例的基础上，引入了uniform统一数据（这里也可以使用varying将数据从顶点着色器传入片元着色器，不过书里没这么用就算了），为点的颜色赋值。（这里偷懒把颜色设置成了随机，没有根据象限赋值）

### 练习于 2018.06.23

### [chapter03_01_MultiPoints](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_01_MultiPoints.html)
使用缓冲区对象，将多个点的坐标传入标签中，调用一次gl.drawArrays来绘制多个点。

（由于webgl是标准归一化坐标到canvas的映射，所以这里全窗口化canvas会呈现屏幕比例的拉伸，由此例题开始修改canvas为正方形以适应示例）

### [chapter03_02_HelloTriangle](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_02_HelloTriangle.html)
通过三个点来绘制三角面。（Face3 -> Triangle，三点确定一个平面）

### [chapter03_03_HelloTriangle_LINES](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_03_HelloTriangle_LINES.html)
绘制线段。

### [chapter03_04_HelloTriangle_LINE_STRIP](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_04_HelloTriangle_LINE_STRIP.html)
绘制连续线段。

### [chapter03_05_HelloTriangle_LINE_LOOP](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_05_HelloTriangle_LINE_LOOP.html)
绘制连续的环线。（首尾相连）

### [chapter03_06_HelloQuad](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_06_HelloQuad.html)
绘制正方形。（两个三角面，带状排列）

### [chapter03_07_HelloQuad_FAN](http://www.wesker926.com/webglProgrammingGuideExercise/chapter03_07_HelloQuad_FAN.html)
绘制飘带。（两个三角面，扇状排列）

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