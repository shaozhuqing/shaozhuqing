```
更换源：
/etc/apt/sources.list
deb http://mirrors.aliyun.com/raspbian/raspbian/ stretch main contrib non-free rpi
/etc/apt/sources.list.d/raspi.list
deb https://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ stretch main ui
1、更换源：
sudo -s
echo -e "deb http://mirrors.aliyun.com/raspbian/raspbian/ stretch main contrib non-free rpi \n deb-src http://mirrors.aliyun.com/raspbian/raspbian/ stretch main contrib non-free rpi" > /etc/apt/sources.list
echo -e "deb http://mirrors.tuna.tsinghua.edu.cn/raspbian/raspbian/ stretch main ui" > /etc/apt/sources.list.d/raspi.list
exit
sudo apt update && sudo apt -y upgrade
2、安装vim
sudo apt-get remove vim-common 
sudo apt-get install -y vim
3、中文输入法
sudo apt-get install ttf-wqy-microhei
sudo apt-get install -y ttf-wqy-zenhei 
sudo apt-get install -y scim-pinyin
sudo apt-get install fcitx fcitx-googlepinyin fcitx-module-cloudpinyin fcitx-sunpinyin
4、开启ssh
sudo service ssh restart
```
