## I/O 端口编址方式

![](http://a1.qpic.cn/psc?/V14YMjxf2CzsRr/NrBG0KpF3EQEf3NYGEmEN50ZQWKwwyW53.tnB6JJLcQet5hdYAjc4JxIzQZ3Xx76TZrB2VlCXsKvx15.BproyQ!!/b&ek=1&kp=1&pt=0&bo=gwNKAQAAAAADJ8k!&tl=1&vuin=3300648086&tm=1590822000&sce=60-2-2&rf=viewer_4&t=5)

### 与存储器统一编址的优缺点

优点：所有访问内存的指令都可以访问I/O端口，不用设置专门的I/O指令；也不需要专用的I/O端口控制信号，简化了系统总线。

缺点：减少了内存地址空间

### 独立编址方式的优缺点

优点：不占用内存空间，而且I/O端口地址线根数少，译码电路简单

缺点：需要专用的控制信号和专用的I/O指令



> I/O端口一次能够传送数据的位数，称为端口位宽。端口位宽有8位、16位和32位几种。



## 基本输入输出接口

输入端口必须具有“通断”控制能力。基本输入接口是一组**三态缓冲器**

上一章：[I/O接口概述]([https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch6/IO%20interface.md](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch6/IO interface.md))

下一章：[数据传送控制方式]([https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch6/Data%20Transmission.md](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch6/Data Transmission.md))

目录：[目录](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/catalog/catalog.md)



