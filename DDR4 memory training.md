---
title: DDR4 memory training
tags: 新建,模板,小书匠
renderNumberedHeading: true
grammar_cjkRuby: true
---

1、training的流程
一般流程是先初始化控制器和phy，然后配置DDR的MR寄存器，然后write leveing、gate-leveing、read-leveing，vref traing，之后是自检，然后才是正式访问

2、ddr4的技术点有
1） CA partity
2） DBI
3）CRC
4）注意3T timing

3、MC-》phy

4、flash
S29GL_128S_01GS_00 这个是pdf文件  spansion  micron flash厂家
1、flash的结构原理图
![enter description here](https://raw.githubusercontent.com/caowangqy/jiaxsj-tu/master/小书匠/1571985491673.png)

2、

3、
设备控制逻辑分成两个部分，一个是HIC，另外一个是EAC，EA代表的是整个读，写，擦等步骤，EAC直接跟memory打交道，而HIC跟主机打交道
EAC负责整个EA的实现

write-buffer 512字节
在program之前，存在一个长度为512字节的write buffer，



