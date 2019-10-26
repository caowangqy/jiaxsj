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




