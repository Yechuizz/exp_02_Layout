# exp_02_Layout
## 1.线性布局
（1）在activit_main.xml中使用LinearLayout布局

（2）要实现目标布局，我采用垂直布局嵌套四个水平布局,一个水平布局包含四个按钮组件

（3）实现按钮均等分，我采用layout_weight，将一行分成“4”份一个按钮占“1”份，关键代码如下

（https://github.com/Yechuizz/exp_02_Layout/pictures/code1.PNG）

（4）实现按钮边框及背景色，我在res的drawble下新建border.xml文件solid android:color="#000000" stroke android:width="2dp" android:color="#999999"分别指定边框大小和边框颜色，在layout中直接用android:background="@drawable/border"即可达到目标效果，关键代码如下

（https://github.com/Yechuizz/exp_02_Layout/pictures/code2.PNG）

（5）实现边框之间距离可以用layout_margin控制按钮与按钮，按钮与父组件间距离，最后效果如下图所示：

（https://github.com/Yechuizz/exp_02_Layout/pictures/exp1.PNG）

## 2.表格布局
（1）在activit_form.xml中使用TableLayout布局

（2）实现下划线效果，我在res的drawble下新建underline.xml文件，采用layer-out，item solid android:color="#666" item android:bottom="2dp" shape solid android:color="#000"分别指定下划线颜色、大小和背景色，在layout中直接用android:background="@drawable/underline"即可达到目标效果，关键代码如下

（https://github.com/Yechuizz/exp_02_Layout/pictures/code3.PNG）

（3）最后效果如下图所示：

（https://github.com/Yechuizz/exp_02_Layout/pictures/exp2.PNG）

## 3.约束布局
（1）在activit_form.xml中使用androidx.constraintlayout.widget.ConstraintLayout布局

（2）约束布局一定要确保水平和垂直方向至少有一个约束

（3）在design中拖动控件建立约束，最后效果如下图所示：

（https://github.com/Yechuizz/exp_02_Layout/pictures/exp3-1.PNG）

（https://github.com/Yechuizz/exp_02_Layout/pictures/exp3-2.PNG）

## 4.问题及解决
（1）在进行约束布局时，利用design拖动控件建立约束比起代码更为方便