# typec_ADXL345
 The prices of raspberry pie is obviously too high🤯
 So  I tried to find other ways to install  klipper 
 Low power Intel processors seem to be a better solution , I got a motherboard from  Waste Market which is equipped with the N3050 processor 
 WOW，look at him ：  Highly integrated . 
![图片](https://user-images.githubusercontent.com/53431902/168425022-f5353120-8198-4d3e-9086-91f06b066501.png)
But PC motherboards don't normally provide SPI for us to use, so we have to use MCU to provide SPI to connect ADXL345
For commercial printers, the schematic diagram of the control panel may not be published and， it's hard to find SPI  pins.
Maybe you got a 3D printer several years ago which means avr was probably the most popular controller of the time, there is no remaining performance to connect an ADXL345
This module integrates stm32f103c6 high-performance ARM MCU (Taobao retail price is about 3 ￥), stm32 ommunicate with ADXL345 and trans data to klipper with usb.
PCB is designed for 0603 components, but unfortunately I lost these treasures, so I had to use 0805 components to cope temporarily😄.
I suggest you use 0603 component if you decide to clone this project 
![图片](https://user-images.githubusercontent.com/53431902/168425228-30f2f151-d220-42e4-b611-f589e2e4b367.png)
This module is suitable for all 3D printers equipped with klipper firmware to achieve resonance measurement, especially for old or commercial machines
 So you see, I succeeded. These are the data 
![图片](https://user-images.githubusercontent.com/53431902/168425281-243704b4-f7d5-4e40-b346-39ddbc3e2d1b.png)
![图片](https://user-images.githubusercontent.com/53431902/168425290-136ecc6d-3f16-4898-ae2f-3a28c459fe0d.png)
