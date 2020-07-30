# LDM6432P5-LED-Control-Driver

## About Library 

This library is forked from LED-Matrix-Display-Driver-Library STM32. The source code to work with . With simple modification, this library can be compatable with more MCUs.

- MCU: NuMaker 131 Uno
    - The driver and gpio is controlled by "NUC131Series_BSP_CMSIS_v3.00.004" and set directly to register. 

- Display size: 64x32
- Color: RGB332
- Hue: 4 each R,G,B
    - If you want to change it to different RGB format or display size. You need to recalculate for buffer size and modify display fuctions.

- If you want SD Card support, you can look at [ChaN's FatFS](http://elm-chan.org/fsw/ff/00index_e.html). 

## How to run example
1. create a directory with the same name as example
2. move all documents inside the directory
3. open .ino and run code

## How to display image?

1. Convert your image file to .bmp
2. Use bmp2h.py to convert to byte array(.h) file
3. Inclue .h file to .iso
4. use displayLoadImage() function

## Adding New Font Style
same as logic displaying image