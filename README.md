# stm32f103-usb-hidmouse
stm32f103 HAL usb hid mouse

## mouse-report[5]

|        | bit7 | bit6 | bit5 | bit4 | bit3 | bit2 | bit1 | bit0 |
| :----: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| byte0  | - | - | - | - | - | MB | RB | LB |
| byte1  | X | X | X | X | X | X | X | X |
| byte2  | Y | Y | Y | Y | Y | Y | Y | Y |
| byte3  | - | - | - | WS | WS | WS | WS | WS |
| byte4  | - | - | - | - | - | - | MW | MW |

LB = Left   Button

RB = Right  Button

MB = Middle Button

WS = Wheel Scroll

MW = Motion Wakeup


more information : ![tutorial-about-usb-hid-report-descriptors](https://eleccelerator.com/tutorial-about-usb-hid-report-descriptors/)

## How to build
connect stlink/stlinkv2 to debug wire pins and
```
make
make flash
```