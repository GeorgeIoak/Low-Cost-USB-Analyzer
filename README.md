# Low Cost High Speed USB Analyzer
This project originated starting from a comment made by Kate Temkin (@ktemkin) with the idea to design a very low cost USB analyzer that was capable of achieving HS (High Speed). The [NXP LPC4357 MCU (32-bit ARM Cortex-M4/M0 MCU)](https://www.nxp.com/docs/en/data-sheet/LPC435X_3X_2X_1X.pdf) can operate at up to 204MHz and has (among other things) a ULPI interface. The [Microchip USB3343](http://ww1.microchip.com/downloads/en/DeviceDoc/USB334x-Data-Sheet-DS00002646A.pdf) is used as the interface between the USB device to test and the LPC4357. The LPC4357 has a 2nd HS USB port that can connect to a PC for USB traffic analysis. The board also includes a 256Mb SDR SDRAM.

In order to keep costs down the size of the board was fixed at 50mm x 50mm and 4 layers. This is far from ideal when doing a controlled impedance design with this many signals so there are some tradeoffs. I didn't want to waste all of the processing capabilities so I managed to bring out ALL of the LPC4357 signals to 1.27mm pitch headers around the perimiter of the PCB. The 24-bit LCD interface signals are all on 1 header and the Ethernet signals are all on another header.

This is NOT a finished project but it is getting close. The design in done in Altium but I am going to try and convert the design to KiCad once it gets closer to being finished

![1](https://github.com/GeorgeIoak/Low-Cost-USB-Analyzer/blob/master/Images/LP4357_SDRAM_3D-Top.png)

![2](https://github.com/GeorgeIoak/Low-Cost-USB-Analyzer/blob/master/Images/LP4357_SDRAM_3D-Bot.png)
