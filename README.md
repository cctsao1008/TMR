TMR-FC : Top Multi-Rotor Flight Controller
------------------------------------------

![TMR-6A](http://api.ning.com/files/jY5mCCMi3CRInh4R8yXGssICRu4ks**VAul7*nLfd2Gr30zyGduX4zLlkqmehdcHnky*z0-FdQ603CA1CuJxyc2YXQpvgG3l/20121231011936.jpg "TMR-6A")

Descriptions
------------


 *  TMR-FC is built for my graduation project, It's designed to control a multi-rotor copter for research,

    It's supposed to not for sale, but if you are interested, you can build it by your self, I can provide

    a empty PCB to you.




 * V1.0

![TMRFC-T](https://lh5.googleusercontent.com/-XYsK7enXFu8/UEcryTjIElI/AAAAAAAAGc8/OJrowpTF_j8/s554/DSC_0192.jpg "TMRFC-T")
![TMRFC-B](https://lh4.googleusercontent.com/-fWInVx9VkrA/UEcrzUAXoeI/AAAAAAAAGdE/_suOKUsVzLk/s554/DSC_0193.jpg "TMRFC-B")

 * V2.0 ( Work stand alone or became a daughter board of Raspberry Pi with camera board for flow application)

![TMRFC-PI](https://lh4.googleusercontent.com/-3GsCG-IL2zc/UkECyNAzdaI/AAAAAAAAPH8/t4znxiEpDLM/w768-h537-no/2013-9-24+%25E4%25B8%258A%25E5%258D%2588+10-30-12.jpg "TMRFC-PI")

 * Raspberry Pi
  
 Offical Website : http://www.raspberrypi.org/

![TMRFC-RPI](https://lh5.googleusercontent.com/-ceNzAmTz5RI/UkEFcuy2-vI/AAAAAAAAPIQ/vlQr_GfAb-8/w590-h369-no/RPi.jpg "TMRFC-RPI")

Resources
---------

 *  DIY Drones Blog :

      [Open Hardware and Software : TMR-FC V1.0](http://diydrones.com/profiles/blogs/my-flight-controller)

 *  User Guide :
 
      [TMR_FC_UM_V1_120730.pdf](http://api.ning.com/files/zkGb0X42pMSBoZSwYeRk3xmjedgHA6iVvhMXisJQ5-8-BqasZVeVXrTL5JO-VfGbOjNi0IqJcKHvWSGABQIJN0GQ00Goep*f/TMR_FC_UM_V1_120730.pdf)

 *  Sechematic :
 
      [TMR_FC_HW_V1_120830.pdf](http://api.ning.com/files/zkGb0X42pMQCmLP*0KVTEsgqDPCMk4Xrd0yNVn0boAruaILcsPhfDeTRqyMbFgaOm*a2DNQkRTxAI7HuhO6A6q*fpwuo6FWx/TMR_FC_HW_V1_120830.pdf)

 *  Gerber :

      [TMRFC_GB_V1_120930.rar](http://api.ning.com/files/jY5mCCMi3CRexrg--zD*nZl6G2gG0jTlRXIGT2z7sKhw3k0wXjNdf-ARRO8cV8KXyBPSvLYKakQJ0EbhTvj45wzjXPB8SEdl/TMRFC_GB_V1_120930.rar)

 *  Software :

      Actually, the software is Porting from "PX4"
      
      [PX4 Autopilot Project](https://github.com/px4)
         
Get source code
---------------

  *  Clone TMR project : 

         pi@raspberry：/x $ git clone [git@github.com:cctsao1008/TMR.git](git@github.com:cctsao1008/TMR.git)
       
         Cloning into 'TMR'...
         remote: Counting objects: 11, done.
         remote: Compressing objects: 100% (10/10), done.
         remote: Total 11 (delta 3), reused 5 (delta 1)
         Receiving objects: 100% (11/11), done.

  *  Initialize and clone submodules : 

         pi@raspberry：/x $ cd TMR/
         pi@raspberry：/x/TMR (master)$ git submodule update --init --recursive
 
         Submodule 'Bootloader' (git@github.com:cctsao1008/Bootloader.git) registered for path 'Bootloader'
         Submodule 'Firmware' (https://github.com/cctsao1008/Firmware) registered for path 'Firmware'
         Submodule 'libopencm3' (git@github.com:cctsao1008/libopencm3.git) registered for path 'libopencm3'
         Cloning into 'Bootloader'...
         remote: Counting objects: 148, done.
         remote: Compressing objects: 100% (50/50), done.

         Receiving objects: 100% (148/148), 52.83 KiB | 19 KiB/s, done.
         Resolving deltas: 100% (96/96), done.
         Submodule path 'Bootloader': checked out 'fd53d28c0760c54e93f230f6aafbc99ee09045dc'
         Cloning into 'Firmware'...
         remote: Counting objects: 80335, done.
         remote: Compressing objects: 100% (16927/16927), done.
         remote: Total 80335 (delta 62860), reused 80332 (delta 62857)
         Receiving objects: 100% (80335/80335), 46.40 MiB | 2.40 MiB/s, done.
         Resolving deltas: 100% (62860/62860), done.
         Submodule path 'Firmware': checked out 'f3fb6509cdf873100c1fe4d0bc379177216c70bc'
         Submodule 'NuttX' (git@github.com:cctsao1008/NuttX.git) registered for path 'NuttX'
         Cloning into 'NuttX'...
         remote: Counting objects: 130874, done.
         remote: Compressing objects: 100% (23609/23609), done.
         remote: Total 130874 (delta 106319), reused 130874 (delta 106319)
         Receiving objects: 100% (130874/130874), 32.98 MiB | 79 KiB/s, done.
         Resolving deltas: 100% (106319/106319), done.
         Submodule path 'NuttX': checked out '56433ad9238ccfd7fe3ba3bd1a050ef785dfaea5'
         Cloning into 'libopencm3'...
         remote: Counting objects: 7300, done.
         remote: Compressing objects: 100% (3341/3341), done.
         remote: Total 7300 (delta 3741), reused 7300 (delta 3741)
         Receiving objects: 100% (7300/7300), 1.61 MiB | 74 KiB/s, done.
         Resolving deltas: 100% (3741/3741), done.
         Submodule path 'libopencm3': checked out '3d3c6d8abf7407f605e0afd1eed533eeb5a3dbb2'

Hardware Features
-----------------

  *  CPU : 

         V1.0
         
             STM32f405RG
             
         V2.0
         
             STM32f407VG

  *  Sensors :

         V1.0
         
             I2C : MPU6050, HMC5883, MS5611
             
         V2.0
         
             I2C : HMC5983, MPL3115A2
             SPI : MPU6000, *LSM303DLM, *L3G4200D
             ADC : *ADXRS620
             
             * Marked are optional item. In some applications, all sensors can be sharing
             to Raspberry Pi for applications to use.

  *  Features :

         V1.0
         
             12 channels PWM output, one PPM input and one Futaba S.BUS input,
             Built-in 10 DOF, 5 LEDs ( controlled by PCA9533/9536), GPS port ( UART / I2C),
             Auxiliary SPI and  GPIO, RF port (APC230 or BT), LiPo Voltage measure via ADC,
             Beeper for tone alarm, SWD port, SONAR, USB VCP and MSC, Micro SD ( can be read via USB),
             Light Bar LED control, Internal FLASH EEPROM emulation using sector 1, 2 and 3 ( 16KB x 3 ),
             RTC ( power keep by 3V CR1220 ), USB OTG,
             ....... etc
         
         V2.0
         
             Under construction, I have ideas, but I do not have money to do, haha, If you want 
             co-work with me or any idea on V2.0, please email, or you want to donate to TMR V2.0.
             
  [![image]](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=chiacheng%2etsao%40gmail%2ecom&lc=US&item_name=TMR%20Project&no_note=0&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHostedGuest)
  [image]: https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif "Donate"

  *  Stress Test VB scripts :

         Auto re-boot loop test, tone alarm loop test, ..... etc

  *  Support PX4 Qupgrade tool :


Firmware update steps
---------------------

### Update bootloader

  * Optinn 1 : Using "dfu-util"  ( Recommend )

         sudo dfu-util -a 0 -d 0x0483:0xdf11 --dfuse-address 0x08000000 -D tmrfc_bl.bin

  * Optinn 2 : Using "Segger J-Link"

      [Segger J-Link EDU official website](http://www.segger.com/j-link-edu.html)

### Update OS image

  * Optinn 1 : Using "dfu-util"

         sudo dfu-util -a 0 -d 0x0483:0xdf11 --dfuse-address 0x08004000 -D tmrfc-v1_default.bin

  * Option 2 : Using "QUpgrade"  ( Recommend )

         Note :  To using "QUpgrade" if you have " tmrfc_bl.bin" been pre-flashed !!! 

         1. Get the tool :  (https://pixhawk.ethz.ch/px4/downloads)<br />
         2. Open "QUpgrade" tool
         3. Select "Advanced"
         4. Select your "tmrfc-v1_default.px4"
         5. Click "Flash"
         6. Connect your TMRFC board via USB, OR click "RESET" key on TMRFC board

  * Optinn 3 : Using "Segger J-Link"

      [Segger J-Link EDU official website](http://www.segger.com/j-link-edu.html)


Finally, Enjoy your TMR-FC !!
-----------------------------


If you need further information or assistance please revert.

Sincerely yours.

TSAO, CHIA-CHENG @NTUT, Taiwan ( chiacheng.tsao@gmail.com )

[![image]](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=chiacheng%2etsao%40gmail%2ecom&lc=US&item_name=TMR%20Project&no_note=0&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHostedGuest)
[image]: https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif "Donate"
