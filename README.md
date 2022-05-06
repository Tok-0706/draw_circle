# draw_circle
## 目的：  编写控制程序，实现小车的绕着圆形轨迹运动；
# 机器人画圆

实验环境：ubuntu 16.04 + ros Kinetic

##  流程：

1、新建工作空间

在ubuntu中打开命令行，输入：

```html
mkdir -p draw_circle/src
cd draw_circle/src
```

如图所示：

<img src="C:\Users\leng\AppData\Roaming\Typora\typora-user-images\image-20220506105423944.png" alt="image-20220506105423944" style="zoom:50%;" />

2、克隆源码

输入：

```c++
git clone https://github.com/Tok-0706/draw_circle.git
```

如图所示：

<img src="C:\Users\leng\AppData\Roaming\Typora\typora-user-images\image-20220506105708837.png" alt="image-20220506105708837" style="zoom:50%;" />

3、 编译

输入：

```
cd ..
catkin_make
```

4、运行仿真环境：

```
source devel/setup.bash
roslaunch my_robot_gazebo view_my_robot.launch
```

如图：

<img src="C:\Users\leng\AppData\Roaming\Typora\typora-user-images\image-20220506110239871.png" alt="image-20220506110239871" style="zoom:50%;" />

![image-20220506110307277](C:\Users\lengqi\AppData\Roaming\Typora\typora-user-images\image-20220506110307277.png)

5、控制小车绕圆形轨迹运动

打开新的终端输入：

```
source devel/setup.bash
rosrun draw_circle draw_circle_node
```

如图：

<img src="C:\Users\leng\AppData\Roaming\Typora\typora-user-images\image-20220506110429190.png" alt="image-20220506110429190" style="zoom:50%;" />

6、结束仿真

在两个终端中分别按下 CTRL + C；
