# Notes on using STM32F103C8T6 Blue Pill 

## Instruction

An easy way to upload the sketches on the Blue Pill under Arduino IDE is installing an [USB HID Bootloader](https://github.com/stm32duino/wiki/wiki/Upload-methods#hid-bootloader-22-hid-bl) as it's done on the Arduino Boards

To install the Blue Pill STM32_HID_Bootloader go to [https://github.com/Serasidis/STM32_HID_Bootloader](https://github.com/Serasidis/STM32_HID_Bootloader)

Suggested to use the the USB converter [https://github.com/Serasidis/STM32_HID_Bootloader#serial-dongle-version](https://github.com/Serasidis/STM32_HID_Bootloader#serial-dongle-version)

The low and medium density STM32_HID_Bootloader file has to be used => [id_generic_pc13.bin](https://github.com/Serasidis/STM32_HID_Bootloader/releases)

To upload the STM32_HID_Bootloader file (id_generic_pc13.bin) an easy way is directly to use the CLI version of STM32CubeProgrammer as done by Arduino IDE

The command under a Linux shell is:

```arduino_STM32/portable/packages/STM32/tools/STM32Tools/1.3.2/tools/linux/stm32CubeProg.sh 1 /tmp/hid_generic_pc13.bin ttyUSB0 -s```


To use the Blue Pill under linux, it is required to install the STM32 HID rules [97-stm32_hid_bl.rules](hardwareliberopinerolo.github.io/Pages/Files/97-stm32_hid_bl.rules) as detailed on [https://github.com/Serasidis/STM32_HID_Bootloader#linux-udev-setup](https://github.com/Serasidis/STM32_HID_Bootloader#linux-udev-setup)


Usefull Links

1. [https://www.electronicshub.org/stm32/](https://www.electronicshub.org/stm32/)
2. [How to Install the STM32 USB Bootloader - Tutorial Video](https://youtu.be/Myon8H111PQ)
