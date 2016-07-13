#ABB机器人介绍

##型号说明
* IRB指ABB标准机器人
* 第1位数字（1,2,4,6）指机器人大小
* 第2位数字（4）指机器人系统

##常见型号
  |型号|臂展|负载|重复定位精度|用途|
  |-----|---|----|-------------|----|
  |IRB1410|1.44m|5kg|0.05mm|焊接|
  |IRB1600|1.2,1.45m|6-10kg|0.02mm|搬运|
  |IRB2400|1.5,1.8m|7-20kg|0.03mm|焊接，切割，搬运|
  |IRB4400|1.95m|60kg|0.19mm|切割，搬运|
  |IRB6620|2.2m|150kg|0.03mm||
  |IRB360|0.8-1.6m|1-8kg||||


##系统
###控制系统
  * S4:			1994-1996年生产的机器人
  * S4C:		1997-1999年生产的机器人
  * S4C plus:	2000-？
  * S5:			？

###应用软件包
RobotWare是ABB机器人应用软件的总称，包含五个系列：
* BaseWare
* BaseWare Option
* ProcessWare
* DeskWare
* FactoryWare



##几个概念
* 热启动：自动检查机器人硬件，正常启动后，保持上次电源关闭时相同的状态。
* 冷启动：系统清盘，系统硬件全面自检


##Controller
IRC5:第五代机器人控制器。
###运动技术
* QuickMode 2:它使机器人在每一步运动具有最大加速度，保证运动周期时间最短
* TrueMove 2：无论机器人运动速度是多少，它保证机器人运动轨迹和编程轨迹一致
* 附加轴：	  最多36个轴

###组成
主电源、计算机供电单元、计算机控制模块（计算机主体）、输入/输出板、Customer 
connections(用户连接端口)、FlexPendant接口（示教盒接线端）、轴计算机板、驱动单元（机器人本体、外部轴）。
![](./img_ABB/servo_system)
A 操纵器（所示为普通型号）B1 IRC5 Control 
Module，包含机器人系统的控制电子装置。
B2 IRC5 Drive Module，包含机器人系统的电源电子装置。在 Single Cabinet Controller 中， Drive Module 包含在单机柜中。MultiMove 系统中有多个 Drive Module。
C RobotWare 光盘包含的所有机器人软件
D 说明文档光盘。
E 由机器人控制器运行的机器人系统软件。
F RobotStudio Online 计算机软件（安装于 PC x 上）。RobotStudioOnline 用于将 RobotWare 
软件载入服务器，以及配置机器人系统并将整个机器人系统载入机器人控制器。
G 带 Absolute Accuracy选项的系统专用校准数据磁盘。不带此选项的系统所用的校准数据通常随串行测量电路板 (SMB) 提供。
H 与控制器连接的 FlexPendant，
J 网络服务器（不随产品提供）。 可用于手动储存： RobotWare成套机器人系统 说明文档在此情况下，服务器可视为某台计算机使用的存储单元，甚至计算机本身！如果服务器与控制器之间无法传输数据，则可能是服务器已经断开！
PC K 服务器的用途：使用计算机和 RobotStudio Online 可手动存取所有的 RobotWare 软件。手动储存通过便携式计算机创建的全部配置系统文件。手动存储由便携式计算机和 RobotStudio 
Online安装的所有机器人说明文档。在此情况下，服务器可视为由便携式计算机使用的存储单元。
M RobotWare 许可密钥。 原始密钥字符串印于 Drive Module 内附纸片上（对于 
Dual Controller，其中一个密钥用于 Control Module，另一个用于 Drive Module；而在 MultiMove 
系统中，每个模块都有一个密钥）。RobotWare 许可密钥在出厂时安装，从而无需额外的操作来运行系统。
N 处理分解器数据和存储校准数据的串行测量电路板(SMB)。对于不带Absolute Accuracy 选项的系统，出厂时校准数据存储在 SMB 上。PC x 算机（不随产品提供）可能就是上图所示的服务器J！如果服务器与控制器之间无法传输数据，则可能是计算机已经断开连接！

###通讯技术
* Robot web services:基于HTML5技术的编程接口使得从任何一台设备都可以和机器人通讯。


