### 28088 与 8086微处理器的功能结构

##### 8088 与 8086 的主要区别

- 在数据总线宽度上，8086 的数据总线宽度为 16 位，而 8088 为 8 位。

- 在内部结构上，两款微处理器都有指令队列，8086 的指令队列长度为 6 字节，而 8088 为4 字节。

##### 8088的结构功能

- 执行单元

  执行单元的主要功能是译码分析指令，执行指令，暂存中间运算结果并保留结果特征。执行单元包括 EU 控制器、算术逻辑运算单元 ALU、通用寄存器组 AX、BX、CX、DX、SP、BP、DI、SI， 专用寄存器、状态标志寄存器等部件，这些部件的宽度都是 16 位。

- 总线接口单元

  总线接口单元包括指令队列、地址加法器、段寄存器、指令指针寄存器和总线控制逻辑。总线接口单元负责 CPU 与内存或输入/输出接口的信息传送，包括取指令、取操作数、保存运算结果。

##### 指令流水线

- EU 和 BIU 两部分按流水线方式工作。

- EU 从 BIU 的指令队列中取指令并执行指令。

- EU 执行指令和 BIU 取指令同时进行，节省了 CPU 访问内存的时间，加快了程序的运行速度。

执行单元和总线接口单元与指令队列协同工作，实现指令的并行执行，提高了 CPU 的利用率，同时也降低了 CPU 对存储器存取速度的要求。

![image-20200530093020824](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200530093020824.png)

### 8080CPU的引脚功能

##### 8088/8086可工作与两种模式

![image-20200530101246059](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200530101246059.png)

##### 8088引脚定义

![image-20200530095605901](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200530095605901.png)

##### 引脚状态及功能

- 最小模式下

![image-20200530100047584](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200530100047584.png)

- 最大模式下

![image-20200530102416839](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200530102416839.png)

##### RESET信号的作用

![image-20200530100527856](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200530100527856.png)