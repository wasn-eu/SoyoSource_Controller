# SoyoSource_Controller
## (c) by [<img src="https://www.pvtex.de/user/themes/darkquark/images/logo/logo_trans.png" width=70>](https://www.wasn.eu)

# All new updates are now under [github://pvtex/SoyoSource_Controller](https://github.com/pvtex/SoyoSource_Controller)

This Controller let you controll all settings of your SoyoSource inverter and can control it for zero grid injection.   
The Software is based on ESP-home and the great work of [syssi](https://github.com/syssi).    
You can find the sources at [github](https://github.com/syssi/esphome-soyosource-gtn-virtual-meter).   
It is based on this [template](https://github.com/syssi/esphome-soyosource-gtn-virtual-meter/blob/main/esp8266-display-display-version-limiter-example.yaml).   

All you have to do is to change the PIN definition:
```
tx_pin_ttl_wifi: GPIO12
rx_pin_ttl_wifi: GPIO13
tx_pin_rs485: GPIO16
rx_pin_rs485: GPIO5
```

And add these lines to activate the status LED:
```
status_led:
  pin: GPIO2
```
    
## external Controller 
in din rail case. needs another adapter cable in the inverter. this adapter cable adds an external connector for the display port.   
![external](../../raw/master/images/soyosource_extern.jpg)      

    
## interal Controller
just take the RS485 board out and plug this in.    
Connect the display port to the board and add the external antenna.     
![internal](../../raw/master/images/soyosource_intern.png)   
   

You can find the gerber files in the directory external or internal.
