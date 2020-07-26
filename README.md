# stm32f103-usb-hidmouse
stm32f103 HAL usb hid mouse

#mouse-report[5]

|        | bit8 | bit7 | bit6 | bit5 | bit4 | bit3 | bit2 | bit1 | bit0 |
| :----: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| byte0  | x | x | x | x | x | x | Middle Button | Right Button | Left Button |
| byte1  | X Axis |
| byte2  | Y Axis |
| byte3  | Wheel Scroll |
| byte4  | Motion Wakeup|


more information : ![tutorial-about-usb-hid-report-descriptors](https://eleccelerator.com/tutorial-about-usb-hid-report-descriptors/)

## How to build
connect stlink/stlinkv2 to debug wire pins and
```
make
make flash
```