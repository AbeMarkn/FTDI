# FTDI
Summarize the information of FTDI topics

221224
0. Check the site of FTDI   https://ftdichip.com/drivers/d2xx-drivers/
1. download two files: Driver (1.4.24, D2xxHelper)
2. See the movie file that is in comment > Video Install Guide
3. copy
   sudo cp / ... /release/build/libftd2xx.1.4.24.dylib .
4. make the symbolic file
   sudo ln -sf libftd2xx.1.4.24.dylib libftd2xx.dylib
5. kill Mac default driver (<-- It's not found on my mac.)
      (kernel) Kext com.apple.driver.AppleUSBFTDI not found for unload request.
      Failed to unload com.apple.driver.AppleUSBFTDI - (libkern/kext) not found.
6. Move to sample folder
7. make
8. sudo EEPROM/read/read
9. See the contents of EEPROM
10. Setting for python (<-- ftd2xx-1.3.1)
   pip install ftd2xx
   

Link:
Bit bung: https://iosoft.blog/2018/12/02/ftdi-python-part-1/
   
D2XX Programmer's Guide: https://ftdichip.com/wp-content/uploads/2020/08/D2XX_Programmers_GuideFT_000071.pdf
