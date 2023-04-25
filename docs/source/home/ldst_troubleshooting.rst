LDST Troubleshooting
====================

Hand Controller Will Not Connect
--------------------------------

.. note:: Complete this checklist first -- stop if reconnected!
  
  - In the handcontroller menu click disconnect
  - Enter settings and select autoconnect
  - Exit handcontroller
  - Restart handcontroller
  
.. warning:: OS Only: Reconnect by Router Reboot
  
  - Shut Down Observing Before Proceeding
  
  - Open 192.168.0.1 in chrome
  - Log into router as blauuwobs@gmail.com
  - Check in Network Map - Wired Clients
  - If MAC address 00-C0-08-96-62-87 is missing or assigned an IP that is NOT 192.168.0.111
    - Click Reboot (Top Right) and Reboot Router
    - When able to reconnect, re attempt connection if not established
  
Persistent Bad Link from Dome Controller
----------------------------------------

.. warning:: Level 5 Only: Reinstall Firmware
  
  - Exit Scopedome
  - Navigate to C:\ScopeDome\Card_Firmware\Arduino\XLoader
  - Launch XLoader
  - Upload Firmware with Settings:
    - Hex File: C:\ScopeDome\Card_Firmware\Arduino\SD_Dome5.4.ino.mega.hex
    - Device: Mega(ATMEGA2560)
    - COM Port: COM40
    - Baud Rate: 115200
