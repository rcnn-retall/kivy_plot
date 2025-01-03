# kivy_plot
A drawing library based entirely on kivy implementation

1. ### LineChartLayout

   + ##### 演示代码

     ![image-20250103162050837](C:\Users\iewv-nyaj\AppData\Roaming\Typora\typora-user-images\image-20250103162050837.png)

     ```python
     body = Polyline_Drawing(meun=True)
     body.plot(x_list=[0,1,2,3,4,5,6],y_list=[12,52,34,43,50,61,24], color=(0,1,0,1))
     body.plot(x_list=[0, 1, 2, 3, 4, 5, 6], y_list=[11, 42, 33, 42, 54, 6, 25])
     ```


   + ##### title(string)

     图表的标题或者名字

     + ##### meun(Boole)

       + True:增加辅助虚线
       + Flase:没有辅助虚线


     + ##### size_hint(tuple)

       + width:比例宽度
       + height:比例高度
       + size(也可以使用)


     + ##### back(list)

       + 图表背景颜色（RBGA）


     + ##### x_name(string)

       + x轴的名字


     + ##### y_name(string)

       + y轴名字


     + ##### pos(tuple)

       + x:x坐标
       + y:y坐标
       + pos_hint(不能使用)


     + #### del_axis(method)

       + axis:删除图表脊骨
         + axis_left (string)
         + axis_right(string)
         + axis_top(string)
         + axis_bottom(string)


   + #### plot(method)

     + 添加折线数据
       + x_list:x轴数据列表（list）
       + y_list:y轴数据列表  (list)
       + color:折线颜色,默认黑色
       + width：折线粗细
