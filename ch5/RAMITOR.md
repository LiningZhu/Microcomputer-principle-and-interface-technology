![img](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/U3..NSiujzLMR7a*2QgXbSWMwZi5Bnnpt.oU2usg7fdaOcuPghJ8VLk2qsZS3lP*q3UcKViqeJsuCaOMnH18iA!!/b&bo=FAKAAQAAAAADB7U!&rf=viewer_4)

- 存储器按其存储介质特性主要分为“易失性存储器”和“非易失性存储器”两大类。

- 其中的“易失/非易失”是指存储器断电后，它存储的数据内容是否会丢失的特性。

<u>由于一般易失性存储器存取速度快，而非易失性存储器可长期保存数据，它们都在计算机中占据着重要角色。在计算机中易失性存储器最典型的代表是内存，非易失性存储器的代表则是硬盘。</u>

### RAM

RAM 是*“Random Access Memory”*的缩写，被译为随机存储器。所谓“随机存取”，指的是当存储器中的消息被读取或写入时，所需要的时间与这段信息所在的位置无关。这个词的由来是因为早期计算机曾使用磁鼓作为存储器，磁鼓是顺序读写设备，而 RAM 可随读取其内部任意地址的数据，时间都是相同的，因此得名。实际上现在 RAM 已经专门用于指代作为计算机内存的易失性半导体存储器。

根据 RAM 的存储机制，又分为**动态随机存储器** ***DRAM***(Dynamic RAM)以及**静态随机存储器 SRAM**(Static RAM)两种。 
DRAM
动态随机存储器 DRAM 的存储单元以电容的电荷来表示数据，有电荷代表 1，无电荷
代表 0，见下图。但时间一长，代表 1 的电容会放电，代表 0 的电容会吸收电荷，因此
它需要定期刷新操作，这就是“动态(Dynamic)”一词所形容的特性。刷新操作会对电容进 
行检查，若电量大于满电量的 1/2，则认为其代表 1，并把电容充满电； 若电量小于 1/2，
则认为其代表 0，并把电容放电，藉此来保证数据的正确性。

![img](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/4pNOqgOvBLvj4yTC9qc55frNeIYO7ZBja8GAqkAprJ1dgBEkSyecUz.c3dGmU**56SVMkTJ.5koodGKnMnin7xIhgAsybnvYQhY6C6X*yG8!/b&bo=FwH*AAAAAAADF9s!&rf=viewer_4)

 ![img](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/U3..NSiujzLMR7a*2QgXbYyC.zt57.MiwgNGuvsJcg1TYY6rnAAEq3xyaQ*Ihmo5Bp9qxxDdAW9XfM.i6vQZDQ!!/b&bo=NAK4AQAAAAADB60!&rf=viewer_4)





![img](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/4pNOqgOvBLvj4yTC9qc55QuXiPSEzb6c9ix1lfoZUtSONNyebEKuExsuG2XZIiu52YM7JY*cLcUY6DjcuW0.xx5nCcJhtWWAObCACIKXDwM!/b&bo=nwL4AQAAAAADJ2Y!&rf=viewer_4)

![img](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/4pNOqgOvBLvj4yTC9qc55Vk3LTa2AtvGttvMXTInYa2OEtu*U46hldrw2o.vO43cKozslfmvD2R8vVIcI9I49NzSC1lnl4xIDWlaCXHLvnc!/b&bo=nAIfAgAAAAADJ4E!&rf=viewer_4)

![img](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/4pNOqgOvBLvj4yTC9qc55StcKS8V3zWbT2muWuSQQVKHC6jzej9vVtsUcskn.zOj9ZsHhV288ECAQqSiqe4KpaZsShva*yYzJF5kuHqocEg!/b&bo=qgK*AQAAAAADJxQ!&rf=viewer_4)

ROM 是“Read Only Memory”的缩写，意为只能读的存储器。由于技术的发展，后来设计出了可以方便写入数据的 ROM，而这个“Read Only Memory”的名称被沿用下来了，现在一般用于指代非易失性半导体存储器，包括后面介绍的 FLASH 存储器，有些人也把它归到 ROM类里边。

![img](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/4pNOqgOvBLvj4yTC9qc55TrusbhmO7muVhVS.UhtjHJyztBz6agkVwKu5yrYBo2lkXvsoDt7tBDa6hQ1mZabEhdJKN3xS1B43J4Oh4*0Jr4!/b&bo=tgK8AAAAAAADFzo!&rf=viewer_4)

FLASH 存储器又称为闪存，它也是可重复擦写的储器，部分书籍会把 FLASH 存储器称为 FLASH ROM，但它的容量一般比 EEPROM 大得多，且在擦除时，一般以多个字节为单位。如有的 FLASH 存储器以 4096 个字节为扇区，最小的擦除单位为一个扇区。

根据存储单元电路的不同，FLASH 存储器又分为 NOR FLASH 和 NAND FLASH。

![img](http://m.qpic.cn/psc?/V13PUOHK2RFsMP/4pNOqgOvBLvj4yTC9qc55UpzYiy7OZsAMoyEz6i.ucaTRvEE.*MyxQUXhIbNgdbW.s.xqIGkF40N4KY0vQ8feHOSXpCysxE6KE15s0l7q3g!/b&bo=0QIRAQAAAAADF*E!&rf=viewer_4)

NOR与 NAND 的共性是在数据写入前都需要有擦除操作，而擦除操作一般是以“扇区/块”为单位的。而 NOR与 NAND特性的差别，主要是由于其内部“地址/数据线”是否分开导致的。

