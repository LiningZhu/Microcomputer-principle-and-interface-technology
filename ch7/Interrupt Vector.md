## 中断向量和中断向量表

8086/8088CPU的中断系统可以处理256种中断，每种中断都有对应的中断服务程序。

### 中断向量

> 中断服务程序的入口地址称为中断向量

### 中断向量表

> 256种中断向量存储在内存中构成一张表，称为中断向量表



每个中断向量都包括两部分：**段基址**和**偏移地址**

存放1个中断向量需要4个内存单元，256种中断向量共需要1k个内存单元，故256k*4=1024M

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/NrBG0KpF3EQEf3NYGEmEN5UnIN3YisOPVhanRguvN2uW.ry96DiSNXjgwEs4jAoDZOkkSoXCxMTwkGtL4YmFDQ!!/b&bo=fANDAQAAAAADBx8!&rf=viewer_4&t=5)

## 硬件中断 

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/NrBG0KpF3EQEf3NYGEmEN6Fey.rW5Ee8pZydMAxOZc1JfET5x*Z5jX1Kqo7OUmCsb2hd1msWE6FJd1wcLaz8vQ!!/b&bo=4wIiAgAAAAADB.M!&rf=viewer_4&t=5)





非屏蔽中断不能被软件禁止，即不受IF标志位控制。

## 中断处理流程

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/jkqgNxaPJb7RsklupiKoXXxFTGQ.LG72Dd3Tn2i2WigFkd0sxypznTdysKQ8WpepRKbqDET2UhFjWsGDkhmoL8Z8MoclO2F4QcW8ojaJe4E!/b&bo=5gJ.AQAAAAADJ5k!&rf=viewer_4&t=5)

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/jkqgNxaPJb7RsklupiKoXe25gtqASR67*RFceokqQZw1RDh7kw*XG*kQDh8w3h1wmjp0bcO5oAmMvzaKfDlHMaeSudF29UP5EgCOiDkjf9o!/b&bo=wAI2AQAAAAADJ*c!&rf=viewer_4&t=5)

### 堆栈的变化

![](http://m.qpic.cn/psc?/V14YMjxf2CzsRr/jkqgNxaPJb7RsklupiKoXUbHUuUhtXwd9XaFfiE5KCf4PsSKXyyuDd8w8v8H*gVdwE5fGlyAqD3mDj9mQ8HCmotev4t2DRzD4A8WFwWE0HQ!/b&bo=0QKbAQAAAAADJ0s!&rf=viewer_4&t=5)



上一章：[什么是中断](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch7/what%20is%20Interrupt.md)

下一章：[8259A的应用](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/ch7/8295A%20Claim.md)

目录：[目录](https://github.com/youmingsama/Microcomputer-principle-and-interface-technology/blob/master/catalog/catalog.md)