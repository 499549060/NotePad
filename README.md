# 基于NotePad应用的功能扩展
## 基本要求
### NoteList中显示条目增加时间戳显示
在NotePad原应用中，笔记列表只显示了笔记的标题。要对它做时间扩展，可以把时间放在标题的下方。
首先，找到列表中item的布局：noteslist_item.xml。要在标题下方加时间显示，就要在标题的TextView下再加一个时间的TextView。但是由于原应用列表item只需要一个标题，所以不需要用上别的布局，要多加一个时间TextView，就要把标题TextView和时间TextView放入垂直的线性布局。<br>
···Java
<!--添加显示时间的TextView-->
    <TextView
        android:id="@+id/text1_time"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:textAppearance="?android:attr/textAppearanceSmall"
        android:paddingLeft="5dip"
        android:textColor="@color/colorBlack"/>
        ···
![](https://github.com/panwenxia/NotePad/blob/master/images/1.png)<br>
### 笔记查询（按标题查询）
![](https://github.com/panwenxia/NotePad/blob/master/images/2.png)<br>
## 扩展功能
### 笔记排序----按创建时间顺序排序
![](https://github.com/panwenxia/NotePad/blob/master/images/3.png)<br>
### 笔记排序----按修改时间顺序排序
![](https://github.com/panwenxia/NotePad/blob/master/images/4.png)<br>
### 导出笔记
![](https://github.com/panwenxia/NotePad/blob/master/images/5.png)<br>
### UI美化
  UI美化主要是让NoteList和NoteSearch每条笔记都有背景色，并且能保存。<br>
![](https://github.com/panwenxia/NotePad/blob/master/images/7.png)<br>
### 背景更换
  将UI美化与背景更换结合，让编辑笔记时的背景色跟笔记列表的该笔记背景色同为一种颜色。<br>
![](https://github.com/panwenxia/NotePad/blob/master/images/6.png)<br>
