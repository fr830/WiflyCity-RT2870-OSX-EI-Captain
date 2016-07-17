# WiflyCity-RT2870-OSX-EI-Captain

This note contain process to bring WiflyCity-RT2870 USB WIFI NIC to run on OSX-EI-Captain and the related files.

Background:
    
    I have a old Wifly-City USB Wireless NIC, but it can not work with my MacBook-Air with OSX EI-Captain. 
    So I search on google and read many articles to find the way to make it work. Finally it works successfully. 
    And I think maybe it is helpful to you with the sample problem, so I record this note.
    
# Process

install network manager

1. run Resources/"1.\ Remove\ workaround\ first.pkg", and restart.
2. run Resources/"2.\ Remove\ old\ files.pkg", and restart.
3. run Resources/"3.\ Install\ 5.4.pkg", DONT RESTART YET.
4. connect the USB wireless nic.

install driver

1. run Resources/Easykext\ Utility.app
2. and drag Resources/RT2870USBWirelessDriver.kext to the window. restart.

disable [SIP](https://support.apple.com/en-us/HT204899)

1. after restart, press "CMD+R" to enter Recovery Mode.
2. Open "Terminal" At “Utilities” menu.
3. Type "csrutil disable".
4. reboot.

finally, the wireless nic will work successfully.





