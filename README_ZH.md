<h3>这是一个toy project，pichulia只是每隔一段时间当我需要一张图片时就把用来创建它的代码放进去</h3>
像素坐标为 `x,y` 当以坐标表示时，左上角为 `(0,0)`，右上角是 `(1,0)`，左下角是 `(0,1)` 。 请务必注意，实际颜色数据为`(y * width + x) * 4 + ~~~`。在变量中，还有一些函数使用 i，j，其中 i 是 y 坐标，j 是 x 坐标。

默认情况下，可以根据需要访问/修改 `Image Class`中的像素数据

`if(img.data[0] == 255)img.data[3] = 127;`

`Image class` 您可以使用它来绘制一个简单的形状

`img.draw_line(~~);`

`img.draw_circle(~~);`

还有一个Painter实用程序，它将在绘制形状时为您提供帮助

`painter.Draw(img, Triangle(), Color());`

如果你实现它，有很多好的功能^-^

可用功能:

* 绘制矩形 `(O(wh))`
* 画一个圆圈 `(O(r^2))`
* 绘制钻石 `(O(r^2))`
* 绘制一条直线 `(O(完整图像))`
* 绘制三角形 `(O(完整图像))`
* 绘制简单多边形 `(O(n*完整图像))`
* 绘制另一幅图像 `(O(max(w1h1, w2h2)))`
* 示例图像

<table>
  <tr><td><p align="center"><img src="./sampleImages/sample1.png" alt="sample1"/></p></td><td><p align="center"><img src="./sampleImages/sample2.png" alt="sample2"/></p></td></tr>
  <tr><td><p align="center">Sample 1 : Red gradient                              </p></td><td><p align="center">Sample 2 : Rectangles + Diamond + Circle             </p></td></tr>
  <tr><td><p align="center"><img src="./sampleImages/sample3.png" alt="sample3"/></p></td><td><p align="center"><img src="./sampleImages/sample4.png" alt="sample4"/></p></td></tr>
  <tr><td><p align="center">Sample 3 : Rectangles + Diamond + Circle only border </p></td><td><p align="center">Sample 4 : Lines                                     </p></td></tr>
  <tr><td><p align="center"><img src="./sampleImages/sample5.png" alt="sample5"/></p></td><td><p align="center"><img src="./sampleImages/sample6.png" alt="sample6"/></p></td></tr>
  <tr><td><p align="center">Sample 5 : Alpha blending and Alpha Behavior         </p></td><td><p align="center">Sample 6 : Load Image                                </p></td></tr>
  <tr><td><p align="center"><img src="./sampleImages/sample7.png" alt="sample7"/></p></td><td><p align="center"><img src="./sampleImages/sample9.png" alt="sample9"/></p></td></tr>
  <tr><td><p align="center">Sample 7 : Whatever you want                         </p></td><td><p align="center">Sample 9 : Triangle and Polygon                      </p></td></tr>
  <tr><td colspan=2><p align="center"><img src="./sampleImages/sample8.png" alt="sample8"/>                                                                          </p></td></tr>
  <tr><td colspan=2><p align="center">Sample 8 : Resize Image                                                                                                        </p></td></tr>
  <tr><td colspan=2><p align="center"><img src="./sampleImages/sample10.png" alt="sample10"/>                                                                        </p></td></tr>
  <tr><td colspan=2><p align="center">Sample 10 : NUI Infographics                                                                                                   </p></td></tr>
</table>

映像 i/o 参考 : https://github.com/nothings/stb

Inital Commit : 2020-03-16 pichulia

Publish github : 2021-06-08 pichulia
