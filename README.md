# WeChatJump
This is WeChat Jump assistant program

Principle:
0.debuge mobile by adb(http://adbshell.com/downloads)
1.get mobile screen capture
2.show screen picture in pc
3.click start position and end position, caculate their distance, covert to push duration time
4.swipe mobile by pc, get new screen capture

Running: demo.wmv

Android Mobile:
1.get root privileges
2.open Developer options(ex: MI Mobile, Setting->About phone->Kernel Version click repeatedly)
3.download Terminal Emulator
   (1)su
   (2)setprop service.adb.tcp.port 5555
   (3)stop adbd
   (4)start adbd
 
 Python:
 pip install Pillow,numpy,matplotlib
 project directory need copy adb
 

 Problem1: Device Unauthorized
 Solution: connect mobile by usb,delete C:\Users\username\.android addkey and addkey.pub(PC), Revoke USB debugging authorization and restart Developer Options(Mobile)
 
 Reference:
 1.http://blog.csdn.net/yelang_110/article/details/55510105
 2.http://blog.csdn.net/gfg156196/article/details/77979507
