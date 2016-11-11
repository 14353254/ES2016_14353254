
##lab05 配置ROS  
###一、配置unbantu仓库过程  
首先配置ubantu的仓库环境，按照https://help.ubuntu.com/community/Repositories/Ubuntu
网址上的指示一步一步进行操作即可  
###二、基本上根据教程就是复制|粘贴，按照顺序执行以下语句，差不多就可以了。不过安装过程很漫长，而且卡的要死，安装的时候可以去干别的事情，然后顺便抬头看一眼电脑看看有没有反应有没有死机==  
1.sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'  
2.sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 0xB01FA116  
3.sudo apt-get update  
4.sudo apt-get install ros-jade-desktop-full  
5.sudo rosdep init  
6.rosdep update  
7.echo "source /opt/ros/jade/setup.bash" >> ~/.bashrc  
8.source ~/.bashrc  
9.sudo apt-get install python-rosinstall  
判断是否配置成功：输入指令roscore，使用ROS的第一件事情就是运行roscore命令，得到下图：  
![ROS配置成功图](https://ooo.0o0.ooo/2016/11/11/58253f610e47f.png)  
###三：实验感想  
没啥感想==讲道理不知道这次实验在干嘛，就是一直在复制粘贴，出错了再重跑，然后百度或者问同学解决问题==
重点是让我们感受一下整个配置过程吧，讲道理也不知道每一条指令在干啥。ROS，全称Robot operation system，
一套框架，底层提供硬件驱动，软件层面支持通用的文件格式。嗯，毕竟硬件太贵，无法切身体会，
那我们就主要体会一下它的仿真功能。嗯，cartographer没有配置，看着群里大家都出一堆问题，然后一安装电脑就卡死，
然后时间也不够，一堆ddl挤在一起，就放弃了==

