# Micro-Autonomous-Quadcopter
Micro quadcopter using [inav](https://github.com/hemkum/inav) as flight controller

# Parts
1. Flight Controller Circuit  
[Eachine Beecore VTX Brushed Flight Controller w/ Betaflight OSD 25mW VTX Smartaudio ](https://www.banggood.in/Eachine-Beecore-VTX-Brushed-Flight-Controller-w-Betaflight-OSD-25mw-VTX-Smartaudio-for-Tiny66x7-p-1305469.html)  
Specs:  
MCU:STM32F303CCT6 (72MHZ, 256K FLASH)  
IMU:MPU6000  
with inbuilt mosfets for coreless motors and other stuff like VTX, OSD  
Datasheet:[[1]](http://img.banggood.com/file/products/20180713045225Eachinebeecorevtx1.0manual.pdf), mirror [[2]]()

2. Frame  
[Oscarliang Whoopie frame for 8.5mm motor, 55mm frame](https://oscarliang.com/whoopee-micro-frame/)  
[Whoopee Micro Quad Build – with Scisky FC](https://oscarliang.com/whoopee-micro-quad-build-scisky-fc/)  
[Whoopie frame stl files](https://www.thingiverse.com/thing:1700311). Source [cad files]()  
[QX90 MINI WHOOP QUAD V2](https://www.thingiverse.com/thing:2137840)  

3. Motor  
Chaoli 8520 coreless [motors](https://www.banggood.in/4X-Chaoli-CL-820-8_5x20mm-Coreless-Motor-for-90mm-150mm-DIY-Micro-FPV-RC-Quadcopter-Frame-p-1069067.html)  

4. Propellers  
Kingkong 65mm [props](https://www.banggood.in/10-Pairs-Kingkong-65mm-Blade-Propeller-Prop-20Pcs-for-720-8520-Coreless-Motor-DIY-Micro-Quadcopter-p-1092166.html)  

5. FPV UVC receiver  
[Eachine ROTG01](https://www.banggood.in/Eachine-ROTG01-UVC-OTG-5_8G-150CH-Full-Channel-FPV-Receiver-For-Android-Mobile-Phone-Smartphone-p-1147692.html)  
It receives video and converts it into USB compatible video format.  

6. Analog to USB video converter  
[Easycap Video capture](https://www.amazon.in/Easycap-Video-Capturing-Device-Directly/dp/B00CI8GO4I)  
It converts analog video to USB compatible video format, it additionally need analog video receiver additionally.  

7. FPV receiver  
[Boscam RX5808](https://www.banggood.in/FPV-Wireless-Audio-Video-Receiving-Module-RX5808-Receiver-p-84775.html?)   
5.8Ghz audio video receiver, format is analog  


# Setup:
Interfacing BMP sensor with f3 board by using UART pins as I2C pins. [Post](https://www.rcgroups.com/forums/showthread.php?2495732-Cleanflight-iNav-%28navigation-rewrite%29-project/page917#post37443443)  
Data from this sensor will be used by flight controller for feedback of height from sea level. It will be fused with data of IMU to hold height etc.
