Introductions :
===================================

### Resources

    1. User Guide :
        TMR_FC_UM_V1_120730.pdf

    2. Sechematic :
        TMR_FC_HW_V1_120830.pdf

    3. Gerber :
        TMRFC_GB_V1_120930.rar

    4. Software :
         The software is Porting from "PX4".
         https://github.com/cctsao1008/TMR

### Hardware Features

    1. MCU : 
          STM32f405RG

    2. AHRS :
          MPU6050, HMC5883, MS5611

    3. Features :
          12 channels PWM output, one PPM input and one Futaba S.BUS input,
          Built-in 10 DOF, 5 LEDs ( controlled by PCA9533/9536), GPS port ( UART / I2C),
          Auxiliary SPI and  GPIO, RF port (APC230 or BT), LiPo Voltage measure via ADC,
          Beeper for tone alarm, SWD port, SONAR, USB VCP and MSC, Micro SD ( can be read via USB),
          Light Bar LED control, Internal FLASH EEPROM emulation using sector 1, 2 and 3 ( 16KB x 3 ),
          RTC ( power keep by 3V CR1220 )
          ....... etc

    4. Stress Test VB scripts :
 
          Auto re-boot loop test, tone alarm loop test, ..... etc

    5. Support PX4 Qupgrade tool :


Firmware update steps :
===================================

### 1. Update bootloader

    sudo dfu-util -a 0 -d 0x0483:0xdf11 --dfuse-address 0x08000000 -D tmrfc_bl.bin

### 2. Update OS image

  * Optinn 1 : Using "dfu-util"

    sudo dfu-util -a 0 -d 0x0483:0xdf11 --dfuse-address 0x08004000 -D tmrfc-v1_default.bin

  * Option 2 : Using "QUpgrade"

    Note :  To using "QUpgrade" if you have " tmrfc_bl.bin" been pre-flashed !!! 

  >  1. Get the tool :  (https://pixhawk.ethz.ch/px4/downloads)<br />
  >  2. Open "QUpgrade" tool
  >  3. Select "Advanced"
  >  4. Select your "tmrfc-v1_default.px4"
  >  5. Click "Flash"
  >  6. Connect your TMRFC board via USB, OR click "RESET" key on TMRFC board

Enjoy your TMRFC !!
