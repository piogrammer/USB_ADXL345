# typec_ADXL345
 As far as I know, raspberry pie is too expensive now, so I can't use raspberry pie to run the klipper control system. Fortunately, however, Intel offers us an additional option, with some Cyan processors offering higher performance while maintaining very low power consumption. I got a motherboard for my advertising machine from my media operator, which is an X86 computer motherboard based on a Saiyang processor. It looks very integrated. 
![图片](https://user-images.githubusercontent.com/53431902/168425022-f5353120-8198-4d3e-9086-91f06b066501.png)
But PC motherboards don't normally provide SPI for us to use, so we have to use MCU to provide SPI to connect ADXL345
For commercial printers, the schematic diagram of the control panel may not be published, and SPI using MCU may not be a viable option
For your old DIY printer, you may use a low-performance AVR single-chip computer, there is no remaining performance to connect an ADXL345
This module integrates stm32f103c6 high-performance ARM single-chip computer (Taobao retail price is about 3 yuan), uses this single-chip computer to operate ADXL345, and transfers data through USB to X86 motherboard
![图片](https://user-images.githubusercontent.com/53431902/168425228-30f2f151-d220-42e4-b611-f589e2e4b367.png)

This module is suitable for all 3D printers equipped with klipper firmware to achieve resonance measurement, especially for old or commercial machines
You don't need to care about the circuit structure of the original machine, you just need to go to Jiali to create the White Lyric PCB and come back to the welding brush program.
 So you see, I succeeded. These are the data 
![图片](https://user-images.githubusercontent.com/53431902/168425281-243704b4-f7d5-4e40-b346-39ddbc3e2d1b.png)
![图片](https://user-images.githubusercontent.com/53431902/168425290-136ecc6d-3f16-4898-ae2f-3a28c459fe0d.png)
