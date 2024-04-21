# Bongo Cat LCD - stm32

This project integrates the [1.8-inch LCD module from Waveshare](https://www.waveshare.com/wiki/1.8inch_LCD_Module#Software_description) with the STM32 board ([NUCLEO-L476RG](https://www.st.com/en/evaluation-tools/nucleo-l476rg.html)).
It displays an interactive Bongo Cat meme that reacts when pressing buttons.

![image](https://github.com/vazonik/stm32-bongo-cat-lcd/assets/46498046/7e5b51dc-1dae-4741-b442-49701160b225)

## Pin Configuration

| STM Pin   | Connected to       | Pin mode            |
| --------- | ------------------ | ------------------- |
| PC3       | DIN                | MOSI                |
| PB10      | CLK                | SCL                 |
| PB6       | CS (Chip Select)   | GPIO_Out            |
| PA9       | DC (Data/Command)  | GPIO_Out            |
| PC7       | RST (Reset)        | GPIO_Out            |
| PA7       | BL (Backlight)     | PWM Timer           |
| PB5       | Left Button        | GPIO_In (Pull-down) |
| PB5       | Right Button       | GPIO_In (Pull-down) |

*(VCC - 3.3V)*
