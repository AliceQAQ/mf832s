# ZTE MF832S Wireless network card

Dependencies:

minicom

modemmanager

usb_modeswitch

ppp



### ArchLinux Users

```bash	
sudo pacman -S minicom modemmanager usb_modeswitch ppp
```

### Debian Users

```bash
sudo apt-get install minicom modemmanager usb-modeswitch ppp
```



### Setup Series port and Baud rate

```bash	
sudo minicom -s

# choose series port setup
# press A for setup series port，/dev/ttyUSB0 normally，press enter for changes
# press E for setup baud rate,press C for choose 9600，enter for yes
# press F for disable the option
# press enter for quit this submenu, choose save as dlf
# Exit from minicom
```



```bash
git clone https://github.com/AliceQAQ/mf832s
cd mf832s
#Notice that maybe you need to execute this command some times.
sudo minicom -S modemconnect
```



### Thanks:

https://www.hissy.cn/2018/07/22/ZTE-MF832-DIAL/

https://blog.csdn.net/qq_42131061/article/details/100125693

