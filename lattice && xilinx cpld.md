---
title: lattice && xilinx cpld
tags: 新建,模板,小书匠
renderNumberedHeading: true
grammar_cjkRuby: true
---

1、lattice  hw上吐出来的文件格式是jed  sw上吐出来的文件格式是vme ；
      xilinx   hw上吐出来的文件格式是bit    sw上吐出来的文件格式是xsvf ；
	  anlogic cpld 暂时没有
	  
2、lattice 的jed文件生成之后，需要使用diamond programmer 另存为.xcf文件，然后使用Diamond Deployment Tool工具，在他的界面中选择
	  Embedded System，然后一路下去，必须选中Fixed Pulse Width（Rev D），最后生成vme文件
	  
3、lattice 的jed文件烧录方法
     1）使用Diamond programmer软件，在标题栏中的Device Properities栏的operation中选择FlASH Erase，Program，Verify，然后点击标题栏的Program按钮，即可完成烧录
	 2）dump 原来的cpld里面的数据方法：
	      在标题栏中的Device Properities栏的operation中选择FlASH Read and Save，然后点击标题栏的Program按钮，即可完成read back操作
		  
4、xilinx的cpld烧录工具是impact，
     1）
	 2）
	 
