## 1.DOL框架描述
***
**Distributed Operation Layer : **The distributed operation layer (DOL) is a software development framework to program parallel applications. The DOL allows to specify applications based on the Kahn process network model of computation and features a simulation engine based on SystemC. Moreover, the DOL provides an XML-based specification format to describe the implementation of a parallel application on a multi-processor systems, including binding and mapping.DOL consists of basically three parts:
* **DOL Application Programming Interface:** The DOL defines a set of computation and communication routines that enable the programming of distributed, parallel applications for the SHAPES platform. Using these routines, application programmers can write programs without having detailed knowledge about the underlying architecture. In fact, these routines are subject to further refinement in the hardware dependent software (HdS) layer.
* **DOL Functional Simulation:** To provide programmers a possibility to test their applications, a functional simulation framework has been developed. Besides functional verification of applications, this framework is used to obtain performance parameters at the application level.
* **DOL Mapping Optimization:** The goal of the DOL mapping optimization is to compute a set of optimal mappings of an application onto the SHAPES architecture platform. In a first step, XML based specification formats have been defined that allow to describe the application and the architecture at an abstract level. Still, all the information necessary to obtain accurate performance estimates is contained.

## 2.DOL配置过程
* **安装一些必要的环境(ubuntu为例)：**    
$	sudo apt-get update  
$	sudo apt-get install ant  
$ sudo apt-get install openjdk-7-jdk  
$	sudo apt-get install unzip      
* 使用$ sudo mkdir dol指令新建**dol文件夹**，使用$ sudo unzip dol_ethz.zip -d dol指令将dolethz.zip解压到dol文件夹中，使用$	sudo tar 
-zxvf systemc-2.3.1.tgz指令解压systemc    
* **编译systemc：**解压后进入systemc-2.3.1的目录下，在终端新建一个临时文件夹objdir并且使用$ cd objdir指令进入该临时文件夹，然后运行configure。  输入sudo make install指令，完成后记录当前工作路径。  
*  **编译DOL：**进入dol文件夹，按照要求修改build_zip.xml文件。然后输入指令$	sudo ant -f build_zip.xml all,约成功会显示build successful  
*  **跑样例：**输入$ cd dol/build/bin/main和$ sudo ant -f runexample.xml -Dnumber=1指令，看最后运行出来的结果，是否successful      
![流程图](https://ooo.0o0.ooo/2016/10/09/57fa5b6c504c3.png)  


## 3.实验心得  
配置这个东西让我想起来上学期被上操作系统实验课时安装虚拟机并配置Ubuntu支配的恐惧，讲真，很多指令已经不记得了，只记得一些cd指令和make指令，所以对我来说，也相当于是从零开始学习配置。果不其然==安装过程很艰辛，配置了两天，一直失败，加上国庆期间又电脑换了系统，尝试了两天，实在成功不了，所以还是用了TA分享的已经配置好的ubantu，感想TA辛勤的付出！！！不知道这个东西有什么用，期待后面的实验。









