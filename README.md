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
