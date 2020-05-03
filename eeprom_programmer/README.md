Original PCB source

http://danceswithferrets.org/geekblog/?page_id=903

arduino sketch and python programmer

https://github.com/petersieg/eeprom

![board](https://github.com/xRA1N/6502/blob/master/eeprom_programmer/20200430130728.jpg)
![board](https://github.com/xRA1N/6502/blob/master/eeprom_programmer/20200430130735.jpg)

Usage

minicom -b 9600 -D /dev/ttyUSB0

Ctrl +A Q leave minicom without reset serial port 
![minicom](https://github.com/xRA1N/6502/blob/master/eeprom_programmer/minicom_no_reset.png)

minicom  -s  file.bin

# -b size (in decimal)              - blank eeprom with 0xff
# -r start end (in decimal)         - read eeprom to terminal
# -s file.bin (programming)         - program eeprom with file.bin
# -v file.bin (verify content)      - verify eeprom with file.bin
# -S file.bin ('smart' programming) - smart programming with file.bin
# -U                                - disable write protection
# -P                                - enable write protection
# -A                                - set parameters for 28C16
# -B                                - set parameters for 28C64
# -C                                - set parameters for 28C256
