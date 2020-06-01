## 动态随机存储器件

先放图

![](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/U3..NSiujzLMR7a*2QgXbTyYSs2m3ENrkjGQcDVaG6YLtZJYJX8149k96KiExy05T58L.3O2OPYg2cbGal.rpg!!/b&bo=lwEdAZcBHQEDCSw!&rf=viewer_4)

要说明的是

RAM与SRAM一样，都是由许多基本存储元电路组成。DRAM的存储元有两种结构，四管存储元和单管存储元。
单管存储元电路如图所示，它由一个MOS管T1和一个电容C构成。当电容C充满电荷，存储元存储的信息为1；电容C中无电荷，存储元存储的信息为0。 
由此可见，DRAM是靠电容存储信息的。集成度高，存储容量大。

------

- 微机中除了8位宽的数据总线，还有16位宽、32位宽、64位宽的数据总线。较宽的数据总线提高了微处理器的数据存取速度。但是微处理器必须能够将任何长度的数据写入存储器，这就带来一系列的问题。比如在32位宽的存储器中如何存取字节型数据？
  微机中16位宽的存储器分为奇偶两个存储体，它既能存储字节宽数据也能存储字类型数据。32位宽的存储器分为四个存储体，字节、字、双字的数据类型都能够存储，64位宽的存储器分为8个存储体，字节、字、双字、四字的数据类型都能够存储。Pentium~core2(64)中使用64位宽的存储器。
  8088/8086有20根地址线，寻址空间是1M。80286、80386SX有24根地址线，寻址空间是16M，80386DX、80486有32根地址线，寻址空间是4G。Pentium~core2可以配置为36根地址线，寻址空间64G，最高可以配置为40根地址线。


#### 电路传送16位的地址到2164。

![](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/U3..NSiujzLMR7a*2QgXbal4R*vNKrJfEK*S.TiN1mLRDLWYXhyUQFt7uVmKnS2qIzCHe*4mgQ*5TniqqL6X5w!!/b&bo=IQJ4ASECeAEDCSw!&rf=viewer_4)

当RAS=0时，A0~A7的信息首先被送到2164芯片的地址引脚上，并锁存到芯片内部的行地址锁存器上。当RAS=1时，A8~A15的信息被送到2164芯片的地址引脚上，由CAS信号将其锁存到芯片内部的列地址锁存器上。
分别称为行地址和列地址，然后利用两个连续的时钟周期将行地址和列地址通过同一组地址线输入到芯片内部。

------

![](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/U3..NSiujzLMR7a*2QgXbe6FdG.HPu*.CIh*HMYEvSB1MOeotAWYwpHg0PvEjoSqTBULcTdd5e72gQTlFVi3Zw!!/b&bo=8gH4APIB.AADCSw!&rf=viewer_4)

- Intel2164的容量为64K×1，（介绍芯片的引脚功能），
- RAS：行选通信号。该信号将行地址锁存在芯片内部的行地址锁存器中。
- CAS：列选通信号。该信号将列地址锁存在芯片内部的列地址锁存器中。
- WE：写允许信号。当它为低电平时，允许将数据写入。反之，当WE=l时，可以从芯片读出数据。
- 芯片内部各存储单元是按照矩阵结构排列的。