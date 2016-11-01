## lab2  DOl实例分析&编程

###任务一：修改 example2，让 3个square square模块变成 2个
**1.1 方法：**修改 xml的iterator，将3改为2  
**1.2 具体操作：**进入examples文件夹中的example2的文件夹，在终端输入指令，cd dol/examples/example2,修改example2.xml,
使用指令sudo gedit example2.xml，弹出窗口，将3改为2，将3个square模块变为2个，输出为i^4，如下图所示：  
![修改后的代码截图](https://ooo.0o0.ooo/2016/11/01/58186d2c1900c.jpg)  
**1.3 运行结果如下**（sudo ant –f runexample.xml –Dnumber=2）：     
![example2截图](https://ooo.0o0.ooo/2016/11/01/58186dbd19a23.png)  
**1.4 DOL图如下：**  
![example2的DOL图](https://ooo.0o0.ooo/2016/11/01/58186e50658df.png)  
  
  
###任务二：修改example1，使其输出3次方数  
**2.1 方法：**修改square.c 在square.c文件中把计算平方的表达式改成计算三次方。  
**2.2 具体操作：**进入到src文件夹，cd dol/examples/example1/src，修改src文件夹中square.c的值，
sudo gedit square.c，将i * i 改为i * i * i，结果图如下,输出为i^3 ，如下图所示  
![修改后的代码截图](https://ooo.0o0.ooo/2016/11/01/58186fbd84c81.png)  
**2.3 运行结果如下**（sudo ant –f runexample.xml –Dnumber=1）：  
![example1截图](https://ooo.0o0.ooo/2016/11/01/58186fbd8012f.png)  
**2.4 DOL图如下：**  
![example1的DOL图](https://ooo.0o0.ooo/2016/11/01/58186fbd72bb6.png)
***
###实验感想：  
本次实验进行的很顺利。因为TA讲的很清楚，还和我们说了应该怎么改，改动的东西很少，所以很简单。重点是了解一些基本内容，还有理解代码里面的内容，
根据要求修改代码。还有进一步的熟悉markdown的规范操作。因为没有获取root权限，所以我不能直接打开文件进行修改，每次都要使用sudo gedit指令对代码
进行修改。
