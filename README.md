# ZTE MF832S无线网卡拨号脚本使用方法

Dependencies:

minicom

modemmanager

usb_modeswitch

ppp



### 对于 ArchLinux用户

```bash	
sudo pacman -S minicom modemmanager usb_modeswitch ppp
```

### 对于Debian系用户

```bash
sudo apt-get install minicom modemmanager usb-modeswitch ppp
```



### 需要先设置串口和波特率

```bash	
sudo minicom -s

# 选择series port setup
# 按A更改串口号，一般是/dev/ttyUSB0，回车结束更改
# 按E更改波特率,按C选择9600，回车结束更改
# 按F关闭该选项
# 回车退出菜单，下移光标保存为dlf
# 选择 Exit from minicom
```



```bash
git clone https://github.com/AliceQAQ/mf832s
cd mfs832s
#注意，此处可能需要多次执行这个命令
sudo minicom -S modemconnect
```

#### 

### 鸣谢:

https://www.hissy.cn/2018/07/22/ZTE-MF832-DIAL/

https://blog.csdn.net/qq_42131061/article/details/100125693

