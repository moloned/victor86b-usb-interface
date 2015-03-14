# USB interface for Victor 86B Digital Multimeter using HIDAPI #

The Victor 86B DMM is cheap and widely available (http://www.dealexcel.com/victor-vc86b-3-34-digital-multimeter_p1985.html) and appears a great match for hobbyist projects.

Unfortunately, however no source code for the DMM app is available for the Victor application http://www.china-victor.com/Files/Download/setup_86b_multi.rar and some of the application's features such as saving to a .csv file do not work.

![http://victor86b-usb-interface.googlecode.com/files/app_screen.png](http://victor86b-usb-interface.googlecode.com/files/app_screen.png)

Although some other software for the Victor 86B is available it is either closed-source (http://homepage.ntlworld.com/green_bean/coffee/roastlogger/dmmdetails.html) or incomplete and written in an interpreted language (http://www.daveansell.co.uk/?q=node/44), therefore it was decided to build a driver program from scratch.

This driver program decodes and displays LCD output from a **Victor 86B USB DMM** data packet that has been accessed using **HIDAPI** http://www.signal11.us/oss/hidapi/ functions.

![http://victor86b-usb-interface.googlecode.com/files/Victor86B.png](http://victor86b-usb-interface.googlecode.com/files/Victor86B.png)

The program decodes and displays output from **Victor 86B USB DMM** based on **HIDAPI** http://www.signal11.us/oss/hidapi/

The tables showings how the USB HID packet (buf) is decoded were reverse-engineered using a bench power-supply and other instrumentation to drive the Victor86B as there is no specification available for the LCD control bits contained in the HID packet.

![http://victor86b-usb-interface.googlecode.com/files/bench-setup.jpg](http://victor86b-usb-interface.googlecode.com/files/bench-setup.jpg)








































