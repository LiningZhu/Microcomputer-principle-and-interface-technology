## 什么是输入输出（I/O）接口

![I/O接口概述](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/NrBG0KpF3EQEf3NYGEmEN*G6I7yK1CGX8KIhv9CBmWrBNfT6WB1OoqbkYmqCj0mv27.5N37SqN80BQX92h993w!!/b&bo=TQMmAgAAAAADB0g!&rf=viewer_4&t=5)

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/NrBG0KpF3EQEf3NYGEmEN*Lfi5FdT23mYrnKhvGR.TpzbxHJEjc*GupUwKBm3BE.IjpMRZQW4XyDEbm3i3Nw.g!!/b&bo=nAWGAQAAAAADBzw!&rf=viewer_4&t=5)

## 输入输出接口功能有哪些

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/jkqgNxaPJb7RsklupiKoXen5nvboa9nWT4A26T3ai9QFj03mGcApXMzqADDf5DBwdyXeAwkgzp1qoTTUjZ*JrwlEsZMM4OTBRSDgeEN7aKE!/b&bo=HAKhAgAAAAADJ78!&rf=viewer_4&t=5)

> 接口应该具有**地址译码**能力

## I/O 接口分类

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/NrBG0KpF3EQEf3NYGEmEN.OQNup7aGmd8cjPfwMnHMECjREpDZ2aEuDCMpw44WaEwOnSg9ip*8cQWMcvQDEJzw!!/b&bo=RwP9AAAAAAADB5s!&rf=viewer_4&t=5)

CPU 与 I/O 接口之间通过系统总线传输信息，包括地址信息、控制信息和数据信息。

## 什么是端口

![](http://a1.qpic.cn/psc?/V14YMjxf2CzsRr/NrBG0KpF3EQEf3NYGEmEN*mzH8a.sMLFVmkq7S7SS70jRGZo2DHvJb0WFVX4UH1hz3nDg0N6flXfIYMZ1a.SXA!!/b&ek=1&kp=1&pt=0&bo=UwJkAAAAAAADFwc!&tl=1&vuin=3300648086&tm=1590804000&sce=60-2-2&rf=viewer_4&t=5)

## 端口分类

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/NrBG0KpF3EQEf3NYGEmEN6.qOXn697xXZ.srdGcoMQhp3G.mCyXJHpGF4kfFeCqbdmiqv5I5SoBpEbHvPk6JMQ!!/b&bo=eQK0AAAAAAADB.0!&rf=viewer_4&t=5)

> I/O 接口在开始工作前，信息存放在控制端口
> 要求输入端口必须具有通断控制能力
> 若外设本身具有数据保持能力，通常可以仅用一个**三态门缓冲器**作为输入接口

> CPU 像输出端口输出数据时，由于外设的速度慢，数据必须在输出端口保持一定的时间使外设能够正确接收，所以输出端口应具备**数据锁存能力**

上一章：[]()
下一章：[I/O 端口编址方式]([https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch6/%E7%AB%AF%E5%8F%A3%E7%BC%96%E5%9D%80%E6%96%B9%E5%BC%8F.md](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch6/端口编址方式.md))
目  录：[目录](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/catalog/catalog.md)