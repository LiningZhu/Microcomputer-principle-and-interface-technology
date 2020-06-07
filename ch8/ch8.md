# 第八章：通用可编程外围设备接口8255A

## 8255A是intel公司生产的可编程<u>并行</u>I/O接口芯片，可用来设计作为单片机与多种外设连接的接口电路，<u>可以扩展3</u>个8位的并行接口。

### 一、8255A的功能结构

#### 1：数据总线缓冲器

#####        D7～D0与系统数据总线相连，负责与CPU进行数据交换。包括输入输出数据、控制字和状态字。

#### 2：读/写控制逻辑

#####        接收来自CPU的地址信息和控制信息。

#### 3：A组控制和B组控制

#####       这两组控制逻辑电路接收来自CPU的控制字，控制两组端口的工作方式及读/写操作。A组控制端口A和端口C的高4位，B组控制端口B和端口C的低4位。

#### 4：端口A、B、C

#####        8255A有3个8位数据输入/输出端口：端口A、端口B和端口C，分别简称为A口、B口和C口。它们对外的引线分别是PA7～PA0、PB7～PB0和PC7～PC0。C口可分成两个4位的端口：C口高4位（PC7～PC4）和C口低4位（PC3～PC0）。

#### 5：8255A可以无条件方式、查询方式和中断方式完成CPU与外设的数据交换

#####         以查询或中断方式工作时，A口与B口可以作为数据输入/输出端口，C口作为握手联络信号，负责输出控制信息或输入状态信息。

### 二、8255A的引脚功能

#### 1：端口地址

#####   8255A包含A口、B口、C口三个独立的数据端口，及一个控制端口。各端口地址如下：

#####             A1A0=00      A口

#####             A1A0=01      B口

#####             A1A0=10      C口

#####             A1A0=11  控制端口

#### 2：8255A的工作方式

#####        8255有三种工作方式：方式0、方式1、方式2；

#####         方式0：

######           （一）基本输入输出方式

​                 （1）适合于三个端口；

​				   （2）A口、C口的高4位、B口、C口的低四位可分别定义为输入或输出，故共有16种组合。

​                 （3）C口可以按位进行置位和复位

######           （二）方式0最适用于无条件传送方式

​                   也能用于查询工作方式，这时可以把C口的高4位定义为输入口，输入外设的状态信号，而将C口的低四位定义为输出口，输出控制信息；这时可用A、B口传送数据；

######           （三）方式0不能工作在中断方式；

#####      方式1：   

######         （一）选通输入输出方式：

​              A口、B口作为数据的输入口或输出口，但数据的输入输出要在控制信号的控制下，控制信号由C口的某些位来提供；

######         （二）方式1适用于程序查询和中断控制方式，它不能工作在无条件传送方式下；

######         （三）方式1选通输出：

​               A口、B口都可以选通输出数据，C口的6条线作为选通控制信号：PC3、PC6、PC7配合A口，PC0、PC1、PC2配合B口；

（四）方式1选通输入

​                 A口、B口都可以选通输入数据，C口的6条线作为选通控制信号：PC3、PC4、PC5配合A口，PC0、PC1、PC2配合B口；

#####     方式2：

######        （一） 双向传输方式，只有A口可以工作在这种方式下。既能发送数据，又能接收数据；它还要利用C口的5条线作为控制信号线； A口的输入输出均具有数据锁存能力，数据的输入输出均可以引起中断；

######        （二）方式2适用于程序查询和中断控制方式。它不能工作在无条件传送方式下。

######        （三）这时B口可以工作在方式0或方式1，C口剩余的3条线可以作为输入输出线或方式1下的控制线

### 三、**查询方式**

![查询方式](http://m.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0wBfyI491*Xb*hJUx7R8gZEZYAk*cxOPGkZLzKZfSbLAlBFxR*X3YcfEPLi1Pdj49g!!/mnull&bo=xAHEAAAAAAADByM!&rf=photolist&t=5)

### 四、**中断方式**

​        （一） 置位PC6，允许中断

​        （二） 等待中断

​        在中断服务程序中发送数据

### 五、控制字

### ![控制字例题](http://m.qpic.cn/psc?/V13qV41h2syAL4/evyMJ*ZwKmN7EwaKYDZ0cLZA5GATNf1KYATViTkUg7T4efaUMGoZUKuxn2DmiTzNpVXkMm0cRc1WuN5fGvd5dNMtSJYtDXoacCHervHZRag!/b&bo=tAOJAgAAAAADFw4!&rf=viewer_4)
![控制字例题](http://m.qpic.cn/psc?/V13qV41h2syAL4/evyMJ*ZwKmN7EwaKYDZ0cMEHlF7*N3ShvAyByy5KPDmAnaQV.1tGd8Ay5epn7oJN7EFZNJOLZzMpaYCOHyuZqme3K591w.NlvUwrTB4ECg8!/b&bo=uAOzAgAAAAADFzg!&rf=viewer_4)

### 六、8255A与微处理器的连接

######         （一） 8255A的D7～D0分别与系统总线的D7～D0相连;

######         （二）RD、WR分别与系统总线的RD、WR信号或者IOR和IOW信号相连（低电平有效）

######         （三）A1、A0分别与系统地址线A1、A0相连;

######         （四） CS由系统地址总线A2~A15译码生成（低电平有效）

######         （五）在PC机中，8255A的I/O端口地址为60H~63H和端口378H~37BH。端口60H~63H用于键盘、扬声器和定时器，端口378H~37BH用于并行打印机（LPT1）端口。

### 七、8255A初始化

#####       8255A初始化，设定端口的工作方式和输入/输出方向，即将方式控制字写入控制端口。

![初始化](http://m.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0xNeGxPKFxii9U*ZMkRjI7EfX2bi*fuTgqeNT.iISYHjmBJentg7zsRfz7QnkEWH6g!!/mnull&bo=kwGSAAAAAAADByI!&rf=photolist&t=5)

## 上一章：[8259A的应用](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch7/8295A%20Claim.md)

## 下一章：[定时器/计数器8253](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch9/ch9-1.md)

## [目录](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/catalog/catalog.md)

