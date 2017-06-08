#WiFi无线门禁考勤系统_PCB

----------------------------------------------------------------------

## 1. 系统介绍

​	本系统采用stm32f103zet6作为控制器，可以刷卡、刷指纹验证用户身份，通过ESP8266 Mesh组网与服务器通讯。

​	服务器端可以添加、删除、修改人员信息，读取设备考勤信息，并输出excel表格。



## 2. 版本更新说明

###   V0.1版

* 初版


### V0.2版

* 修正DS1307电源电压为5V
* 修正指纹模块接口滤波钽电容的极性
* 将蜂鸣器接口从PE5更换到PA0，方便用定时器控制无源蜂鸣器
* 将DS1307 OUT端口连接到PE6，方便使用中断读取时间
* ESP8266 GPIO4连接到PF7，GPIO5连接到PB1，方便使用双线透传SPI功能
* 将TF卡槽从翻盖式改为弹出式

### V0.3版

- 添加EE Bang 字符
- 将门外液晶插口翻转，方便排线插入