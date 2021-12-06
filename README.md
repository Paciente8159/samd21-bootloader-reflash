# samd21-bootloader-reflash
Reflashing SAMD21 using a STM32F103-Bluepill has a CMSIS-DAP.
If you are like me you must have already loaded firmware from the SAMD21 Wemos about the bootloader because you forgot to save with offset 0x2000.
This is a collection of scripts and firmware that helps to restore your Wemos back to it's former state using a STM32F103-Bluepill.

# dependencies
First you need to have openocd on your PC. Add it to your PATH or simply place these files in the same path of openocd.exe

# firmware
The CMSIS-DAP firmware was based on this [site](http://wiki.geniekits.com/usb_express/cmsis-dap)

# using
Burn the provided CMSIS-DAP firmware to your bluepill (using STLink or other programmer)
Connect Bluepill pin B11 to Wemos SWDIO and Bluepill pin B10 to Wemos SWCLK. and plug both boards to USB.
![Wemos](https://github.com/Paciente8159/samd21-bootloader-reflash/blob/main/samd21-uno-wemos-top.jpg)
![Bluepill CMSIS-DAP](https://github.com/Paciente8159/samd21-bootloader-reflash/blob/main/dap-to-target.png)
Just run the bootloader.bat file and you should be done after ir finnishes.
