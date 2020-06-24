#### （一）

- ##### 微处理器通过【总线】与存储器和外部设备进行数据交换。

- ##### 8086CPU能访问的最大存储容量是【1M】。

- ##### 存储器是计算机的存储和记忆部件，用来存放【数据】和【程序】。

- ##### 总线是计算机系统中互连各部件的一组【公共】信号线，负责各部件之间的信息传递。

- ##### 根据信息的类别，系统总线又分为【数据总线】、【地址总线】、【控制总线】。

#### （二）

- ##### 进制转换

- ##### BCD码就是用二进制编码表达的【十进制数】

#### （三）

- ##### 8086和8088CPU都是【16】位的微处理器

- ##### 8086/8088CPU内部按功能被分成两大组成部分，一个是【执行单元 EU】，另一个是【总线接口单元 BIU】

- ##### 8086CPU数据总线的宽度是【16】位，8088CPU数据总线宽度是【8】位。

#### （四）

- ##### 8088CPU一共有【20】根地址线，数据总线一共有【8】根。

- ##### 双列直插的8088CPU有【2】个电源地引脚。

- ##### 双列直插的8088CPU的VCC引脚是【5V电源正】引脚。

- ##### 8088CPU的最小工作模式和最大工作模式由【MN/MX*】引脚决定。

- ##### 双列直插的8088CPU的ALL引脚提供的是【地址锁存信号】。

- ##### 8088CPU的INTR引脚的功能是【外部中断请求信号】。

##### （五）

- ##### 微处理器各引脚信号在时间上的先后顺序关系被称为【时序】。

- ##### 微处理器一般有两种度量方法，一种是【时钟周期】，另一种是【总线周期】。

- ##### CPU通过【总线】进行一次读/写所需要的时间称为一个总线周期。

- ##### 每个时钟脉冲持续的时间被称为【时钟周期】，是计算机内部最小的时间单位，8088CPU的一个标准总线周期包含【4】个时钟脉冲。

- ##### 8088CPU在最小工作模式下，总线信号全部由【CPU】来控制。

- ##### 8282芯片组是带三态输出的8位【锁存器】。

#### （六）

- ##### 8088CPU存储器的寻址空间为【1M】，8088CPU利用分段管理的方法对存储空间进行划分和管理，每一段的最大空间为【64k]。

- ##### 8088CPU为了能用16位的寄存器存储20位物理地址，把物理地址分成【段地址】和【偏移地址】的形式分别存储在2个16位的寄存器中，8088CPU有【4】个段寄存器。

#### （七）

- ##### 标志寄存器的标志共分为2类，一类是状态标志，一类是【控制标志】。

- ##### 奇偶标志位【PF】，运算结果是0的标志位【ZF】。堆栈指针寄存器【SP】，指令指针寄存器【IP】。

- ##### 为了能访问1k*8位存储空间的每一个字节，得需要【10】根地址线。

  ##### 一个1k*8位的存储器，地0个字节的地址是0，那么他的最后一个字节的地址是【3FFF H】

  ##### 通常用3FF H表示1k存储区域，用7FF H表示2k存储区域，用FFF H表示4k存储区域，用FFFF H表示64k存储区域，FFFF H=1M。

#### （八）

- ##### 静态存储器的特点有:【存取速度快】，【不需要刷新】，【功耗大】，【以双稳态触发器为基本存储电路板】

- ##### 地址译码的方法有【全地址译码】和【部分地址译码】

- ##### 【全地址译码】就是把系统中全部地址线与芯片相连，其中高位地址线经过译码电路译码后作为芯片的片选信号；低位地址线与芯片中的相应地址线一对一连接。

##### ![](http://m.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFQaLeHEGEDpTZNgtFaJzL5wbpxzyHCCJvmZlpBwqDhClYUHUlHixPzKLirYwgKq9HQ!!/mnull&bo=NgQ2BjYENgYRCT4!&rf=photolist&t=5)

​                                        

##### ![](http://m.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFYa23s7XvJNtGUtF.4ZdMWJ2CsZCnrdBppw.mWsQZBoZBMXsZWHkAnBN6rEhW6p5wQ!!/mnull&bo=OARYBjgEWAYRCT4!&rf=photolist&t=5)

#### （九）

- ##### 动态随机存储器在工作的过程中，要不断的对其存储内容进行【刷新】，要不然数据就会丢失。

- ##### 电可擦除存储器的英文符号为【EEPROM】

- ##### Cache实体的本质是一块【SRAM】存储器

- ##### Cache对程序员来说【是不可见的】

- ##### Cache工作是基于程序和数据访问的【局部性】原理

#### （十）

- ##### I/O接口的功能包括：【地址译码】，【数据传送】，【数据格式转换】，【信号电平转换】，【提供握手联络信号灯】

- ##### CPU通过给接口分配地址来识别接口，并通过地址总线将地址信息传送给接口，所以接口应该具备【地址译码】的能力

- ##### 按照数据的传送方式，I/O接口可分为【并行接口】和【串行接口】两大类

- ##### 在I/O接口电路需要设置若干专用寄存器，用来缓冲输入输出数据、设定控制方式、保存输入输出状态信息等，这些寄存器科呗=被CPU直接访问，我们通常称其为【端口】，端口可以分为【数据端口】、【状态端口】、【控制端口】

- ##### ![](http://m.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFSDCQrMidF72nU4f*gzNTBpdHl3TCgVhN6kFdmrF1fMsxKP.vZ8k.9z2IWW55I7uDA!!/mnull&bo=OASaATgEmgERCT4!&rf=photolist&t=5)

【锁存】

- ##### ![](http://m.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFdUcBZ.ATg9IMJIipdDG5S6yOfpvd7t5EAKvM9ALKKBYeXXRyoQEOplQ7Al1gHFkXQ!!/mnull&bo=OAR7AjgEewIRCT4!&rf=photolist&t=5)

【独立编址】【独立编址】

- ##### ![](http://m.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFTAcJIUmU5*fu7WPqr.CUg4jOLH9.*gU5Hw6Z4GmwDDzHSGp12FoFyByB196E0UkBg!!/mnull&bo=OAQ3BTgENwURCT4!&rf=photolist&t=5)

#### （十一）

- ##### ![](http://m.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFX3kq*pmblALiRktLQmQnmbuJnp5MkvLpR4ulcQhYKt3h6Go2PPWaIEdUYqR5YZulQ!!/mnull&bo=OASFBDgEhQQRCT4!&rf=photolist&t=5)

##### 描述：当控制端为低电平时，数据从A端输入，Y端输出；当控制端为高电平时，三态门呈高阻状态，，A端与Y端断开。

- ##### ![](http://m.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFaLXLG7edLlFbnxTfCtWyC24Hzc75GyiGDBXVq*yGDs*2nXkBkdsYziPRrz3SpSZCQ!!/mnull&bo=OARDBDgEQwQRCT4!&rf=photolist&t=5)

##### 描述：CPU在读取8个开关状态时，会执行一条IN指令：IN AL,PORT。指令里的PORT就是端口地址。端口地址经过译码，产生片选信号为低电平，IN指令在执行过程中产生读信号为低电平，经过或门为低电平。74AL的8个开关三态门就打通了，8个开关的状态数据就到了数据总线上。CPU在数据总线上接收数据并把它存到AL寄存器中。

- ##### ![](http://m.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFVIW8dLh3up01gZeJaw3Zsanr4vakT4S9h0vRYukigL8cyQZ55SDZLOmhcU*XJZjjw!!/mnull&bo=OAREBDgERAQRCT4!&rf=photolist&t=5)

【55H】

#### （十二）

- ##### 识别键盘哪个键被按下的过程中称之为【键盘扫描】，对于机械按键一般要演示==延时去抖动，才能确认键盘是否按下。

- ##### 【中断】是指在程序执行过程中，出现某种紧急事件，CPU暂停当前执行的程序，转去执行处理该事件的程序，执行完后返回被暂停的程序继续执行的过程。

- ##### 中断源大体可分为两类：CPU内部产生【内部中断】，其他为【外部中断】

- ##### ![](http://a1.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFa833GZU8dC5LyDpTPMdWU8TE15yHuw9e7VQPce4vDUM4*EUh3p0vsFBrHCE6Gk2OA!!/c&ek=1&kp=1&pt=0&bo=MgTeBDIE3gQRGS4!&tl=3&vuin=2715451910&tm=1591016400&sce=60-2-2&rf=0-0)

【AF/AF H/F5/F5 H】

- ##### 中断处理的基本过程包括哪五个阶段，请描述：

  ##### 程序判断中断优先级的高低，设置断点保护，再进行中断程序的调用，中断完成，返回原程序继续执行。

  ##### 大致就是：中断请求 中断响应 中断处理 中断返回

- ##### 中断响应过程包括哪四个阶段，请描述：

  ##### 1、保护断点，即保存下一将要执行的指令的地

  ##### 	  址，就是把这个地址送入堆栈。
  
  ##### 2、寻找中断入口。
  
  ##### 3、执行中断处理程序。
  
  ##### 4、中断返回，执行完中断指令后，就从中断处
  
  #####       返回到主程序，继续执行。

#### （十三）

- ##### ![](http://a1.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFTaiKkrGpBsDvYgyHnNltHuG15u8AtJknwTZKCCuuIm9VtgkfL0aTFRYa6SdQPTN8A!!/c&ek=1&kp=1&pt=0&bo=OASiBDgEogQRGS4!&tl=3&vuin=2715451910&tm=1591016400&sce=60-2-2&rf=0-0)

##### 描述：CPU首先了解外设的状态在“忙”还是“闲”。一般外设会送出一个ready信号到状态端口，有信号ready则为逻辑1，否则为0。输入设备准备好数据后会发出一个选通信号，选通信号完成两个功能，一是把准备好的数据选入锁存器，二是告诉CPU已经把数据准备好了。

##### 地址总线经过译码后，打开三态门缓冲器，此时外设送来的准备好信号就经过三态门缓冲器送到数据端口，数据总线判断ready信号。不同地址经过译码，经过门电路处理对ready信号复位，锁存器内容就可以送到数据总线上。

##### （十四）

- ##### 8086/8088CPU在获得中断类型码后，会转入中断处理过程，在这个过程中直至中断完成，会处理的七件事：

  ##### 1.标志寄存器的内容入栈

  ##### 2.清除中断标志IF和TF

  ##### 3.CS的内容入栈

  ##### 4.IP的内容入栈

  ##### 5.根据中断类型码，在中断向量表中取出中断向 量装入IP和CS
  
  ##### 6.执行中断服务程序
  
  ##### 7.中断返回
  
- ##### 一个8259A芯片可以管理【8】个中断源。

- ##### 在8086/8088微机中，当中断被响应，CPU获得的中断类型码是由【8259A】送来的。

#### （十五）

- ##### 8255A是inter公司生产的可编程【并行】I/O接口芯片，可用来设计作为单片机与多种外设连接的接口电路，它可以扩展【3个】8位的并行接口。

- ##### 8255A工作在方式1模式下，需要【C】口来配合其他端口工作。

- ##### 8255A工作方式选择控制字有【2】个，它们通过控制字的【最高位】来判断是哪一个控制。

#### （十六）

- ##### 8253是intel公司生产的可编程【定时/计数】芯片，它内部有【3】个功能完全独立的【16】位计数器

- ##### 8253的启动可以由软件来启动，也可由外部信号来启动，由外部信号启动的方法又称为【硬件】启动

- ##### 8253的有【6】种计数方式

- ![1](http://m.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0x3K*opgs42vGR.Fb6fND6*qWMc07t56sMYQV2IuM*C6UveQLWRSgcmZ7CKMXP.U.w!!/mnull&bo=DwSHAg8EhwIRBzA!&rf=photolist&t=5)

  ##### 上图是8253的初始化及工作过程各信号示意图，从图中我们可知，计数初值是【4】，技术完毕后OUT端输出【高】电平信号作为提示信号或作为中断信号

#### （十七）

- ##### ADC(A/D)的功能是将【模拟量】转换为【数字量】，而DAC的作用正好相反

- ##### D/A转换器的【转换时间/建立时间】是指输入数字量变化时，输出电压变化到相应稳定电压值所需要的时间

- ##### DAC0832是一个【并行】的【8】位的DA转换器，其电流建立时间约1us

- ##### DAC0832的转换输出结果形式是【电流型】

- <img src="http://a1.qpic.cn/psc?/V11jp7Fm32qabE/W6D0nDePuU8z.mGR2KhyFTHScP95gxQEZ00OGln5AxpeM3qodygG4dpN506qFlCVsJO2PC.XXsYuYRk2O5HdXQ!!/c&amp;ek=1&amp;kp=1&amp;pt=0&amp;bo=OAS0BDgEtAQRGS4!&amp;tl=3&amp;vuin=2715451910&amp;tm=1591794000&amp;sce=60-2-2&amp;rf=0-0" style="zoom: 67%;" />

##### 5V电压

##### LE1=1或LE2=1时，另一个寄存器处于受控状态，执行一次写操作，就开始转换。

### 链接

目录：[目录](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/catalog/catalog.md)

