# 这个仓库用于储存阅读[《webgl Programming Guide》](https://sites.google.com/site/webglbook/)时，所写的随章节练习项目。

#### 好记性不如烂笔头，敲一遍比什么都强。

### [chapter2_1_HelloCanvas](http://www.wesker926.com/webglProgrammingGuideExercise/chapter2_1_HelloCanvas.html)
设置颜色缓冲区清除颜色，并清除画布。

### [chapter2_2_HelloPoint1](http://www.wesker926.com/webglProgrammingGuideExercise/chapter2_2_HelloPoint1.html)
绘制一个点，像素大小10.0，颜色红。

### [chapter2_3_HelloPoint2](http://www.wesker926.com/webglProgrammingGuideExercise/chapter2_3_HelloPoint2.html)
和上个示例一样，不过使用了attribute标签将点的坐标从webgl系统外部赋予。（自行修改了部分，生成100个点）

### [chapter2_4_ClickedPoints](http://www.wesker926.com/webglProgrammingGuideExercise/chapter2_4_ClickedPoints.html)
设置交互内容，点击鼠标，在目标位置生成一个点。

### [chapter2_5_ColoredPoints](http://www.wesker926.com/webglProgrammingGuideExercise/chapter2_5_ColoredPoints.html)
在上一个示例的基础上，引入了uniform统一数据（这里也可以使用varying将数据从顶点着色器传入片元着色器，不过书里没这么用就算了），为点的颜色赋值。（这里偷懒把颜色设置成了随机，没有根据象限赋值）
