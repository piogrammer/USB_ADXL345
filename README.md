# typec_ADXL345
本方案的使用教程https://www.bilibili.com/video/BV1ou411z7Yv/
在Klipper打印控制系统中，我们可以使用一个X86主板安装ubuntu然后将klipper运行在这里
一个低功耗的X86电脑主板如下图
![图片](https://user-images.githubusercontent.com/53431902/168425022-f5353120-8198-4d3e-9086-91f06b066501.png)
但，电脑主板一般不对外提供spi给我们使用，所以，我们必须使用MCU的spi来连接ADXL345
对于商品打印机，控制板的原理图可能并不会公布，使用mcu的spi可能是一个无法行得通的办法
对于自己diy的老旧打印机，可能使用了低性能的AVR单片机，没有剩余的性能以连接一个ADXL345了
这个模组，集成了stm32f103c6高性能ARM单片机（淘宝零售价3元左右），使用此单片机对ADXL345进行操作，并将数据通过USB传输给X86控制板
![图片](https://user-images.githubusercontent.com/53431902/168425228-30f2f151-d220-42e4-b611-f589e2e4b367.png)

本模组适用于所有搭载了klipper固件的3d打印机，以实现共振测量，特别适合于老旧机器或者商品机改造
不需要关心原来机器的电路结构，只需要去嘉立创白嫖PCB然后回来焊接刷入程序即可

数据展示
![图片](https://user-images.githubusercontent.com/53431902/168425281-243704b4-f7d5-4e40-b346-39ddbc3e2d1b.png)
![图片](https://user-images.githubusercontent.com/53431902/168425290-136ecc6d-3f16-4898-ae2f-3a28c459fe0d.png)
