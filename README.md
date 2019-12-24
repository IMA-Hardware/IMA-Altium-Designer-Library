IMA-Altium-Designer-Library
==============
广东工业大学IMA蛋协AD封装库
--------------

由广东工业大学智能硬件与互联网创业协会硬件部维护，引用须注明出处，欢迎大家提交Pull request，若为蛋协硬件部干事，可向部长申请加入项目开发小组（提交个人邮箱）

## 1. 使用说明
将根目录下的IntLib文件夹中的库复制到你的库文件夹中，在AD中安装即可使用（推荐），也可以直接导入


## 2. 文件目录说明：

- ☆常用芯片的封装☆ ：常用的PCB封装，带3D模型，自制库时请优先选用其中的pcb封装

- 1.Base ：基础封装——电阻（可变电阻等都在里面）、电容、电感

- 2.Connector ：连接件封装
    - Miscellaneous Header ：2.54mm、1.27mm排针
    - Miscellaneous Connectors ：未归类的连接件

- 3.Socket ：插座封装

- 4.Transistor ：二极管（LED在里面） 三极管 MOS管

- 5.XTAL ：晶振封装

- 6.Relay ：继电器封装

- 7.Fuse ：保险丝封装

- 8.Switch ：开关封装

- 9.IC ：芯片封装
    - Miscellaneous MCU ：单片机封装
    - Miscellaneous IC ：IC封装（除了在下面的那些细分分类）
    - Miscellaneous Digital IC ：数字IC封装
    - Miscellaneous PMIC ：Power Manage IC 电源管理IC

- 10.Model ：模块封装

- 11.Display ：显示模块
    - Miscellaneous LED Segment Displays ：数码管封装
    - Miscellaneous LCD ：屏幕封装

- 12.Others ：其他（目前只有测试点封装）

- IntLib ：所有库的编译集合（除了Connecter内未归类的连接件封装）

## 3. 开发步骤说明

1. Fetch origin 查看更改，如果有就pull下来
2. 浏览一下近期的commit history
3. 打开想更改的库文件夹，打开对应的.LibPkg库包工程
4. 编辑
5. 编译当前的库包工程，并检查错误
6. 在Project Output文件夹中找到打包好的IntLib文件，复制一份到根目录的IntLib中
7. 写commit comment，内容要求包括更改的库名称与添加的元器件或封装，如：“add Micro-USB Type-C into Socket library”