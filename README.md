[![Build Status](https://travis-ci.com/hanwckf/rt-n56u.svg?branch=master)](https://travis-ci.com/hanwckf/rt-n56u)
![GitHub All Releases](https://img.shields.io/github/downloads/hanwckf/rt-n56u/total)
[![release](https://img.shields.io/github/release/hanwckf/rt-n56u.svg)](https://github.com/hanwckf/rt-n56u/releases)

# README #

### UI预览 ###
[![50MtR1.png](https://z3.ax1x.com/2021/10/19/50MtR1.png)](https://imgtu.com/i/50MtR1)

### 宝塔纯净版介绍 ###
* 基于BT官方剥离了所有与BT官方的通信、上报、下发；
* 所有功能与原版一致，不会有任何异常，如有任何问题请参考宝塔官方解决方案；
* 提升为企业会员，软件商店中的所有[运行环境]、[免费插件]、[宝塔插件]、[专业版插件]、[企业版插件]；部分[第三方应用]安装可能会失败。

### 脚本来源1 ###
* 安装要求
内存：512M以上，推荐768M以上（纯面板约占系统60M内存） 硬盘：100M以上可用硬盘空间（纯面板约占20M磁盘空间） 系统：CentOS 7.1+ (Ubuntu16.04+.、Debian9.0+)，确保是干净的操作系统，没有安装过其它环境带的Apache/Nginx/php/MySQL（已有环境不可安装） ### NEW端口：8888

安装脚本
Centos 安裝腳本 面板端口：8888

yum install -y wget && wget -O install.sh https://download.fenhao.me/install/install_6.0.sh && sh install.sh
試驗性 Centos/Ubuntu/Debian 安裝命令 獨立運行環境（py3.7） 可能存在少量兼容性問題 不斷優化中

curl -sSO https://download.fenhao.me/install/install_panel.sh && bash install_panel.sh
Ubuntu/Deepin 安裝腳本

wget -O install.sh https://download.fenhao.me/install/install-ubuntu_6.0.sh && sudo bash install.sh
Debian 安裝腳本

wget -O install.sh https://download.fenhao.me/install/install-ubuntu_6.0.sh && bash install.sh
Fedora 安裝腳本

wget -O install.sh https://download.fenhao.me/install/install_6.0.sh && bash install.sh
Linux 面板 7.5.1 升級命令（已安裝面板或舊版本或免費版升級專業版）

curl https://download.fenhao.me/install/update6.sh|bash

### 脚本来源2 ###
宝塔 7.6.0版本 [推荐/稳定版本]

Centos全新安装命令：根据系统执行框内命令开始安装（大约2分钟完成面板安装）升级后可能需要重启面板
yum install -y wget && wget -O install.sh http://v7.hostcli.com/install/install_6.0.sh && sh install.sh
Ubuntu/Deepin全新安装命令：
wget -O install.sh http://v7.hostcli.com/install/install-ubuntu_6.0.sh && sudo bash install.sh
Debian全新安装命令：
wget -O install.sh http://v7.hostcli.com/install/install-ubuntu_6.0.sh && bash install.sh
Fedora全新安装命令:：
wget -O install.sh http://v7.hostcli.com/install/install_6.0.sh && bash install.sh
已经安装官方面板，执行下列命令升级到7.6.0纯净版：
curl http://v7.hostcli.com/install/update6.sh|bash
其他非官方版本(含开心版、快乐版、纯净版等 7.4.5至7.6.0版本之间所有版本均可)，执行下列命令升级到7.6.0纯净版：
curl http://v7.hostcli.com/install/update6.sh|bash
任意非官方版本还原到官方最新版
curl http://download.bt.cn/install/update6.sh|bash

### 特别说明 ###
* 1.该项目只是收集网上的开源项目用于本地虚拟机测试以及小白建站测试，请不要使用于违法途径
* 2.开源无情人有情，请不要滥用或者出售脚本，让脚本制作的大佬遭受不白之冤
* 3.脚本不一定什么时候就没了，记得及时建立快照


***

### 固件特点 ###
- 使用[gorden5566](https://github.com/gorden5566/padavan)的汉化字典
- [aria2](https://github.com/aria2/aria2)可选使用较新版本的预编译程序 ```CONFIG_FIRMWARE_INCLUDE_ARIA2_NEW_PREBUILD_BIN```
- aria2前端更换为[AriaNg](https://github.com/mayswind/AriaNg)
- [curl](https://github.com/curl/curl)可选编译可执行程序```CONFIG_FIRMWARE_INCLUDE_CURL```
- 使用了[PROMETHEUS](http://pm.freize.net/index.html)提供的部分补丁，包括新版本的类库、软件包和WIFI驱动补丁
- 使用了[Linaro1985/padavan-ng](https://github.com/Linaro1985/padavan-ng)的部分软件包
### 固件管理 ###
- 我编译的固件后台管理地址:
```shell 
10.32.0.1 
user: admin
password: admin
```

- 已额外适配除官方适配外的以下机型
>- MI-3 (USB)
>- MI-3MI (USB) ```小米路由3硬改SOP flash 16mb```
>- MI-3A
>- MI-3C
>- MI-4C
>- MI-4A-100M
- 小米路由3C 网口以及LED灯配置分别如下
>- wlan and lan: >>>>> kernel-3.4.x.config
```shell
# CONFIG_RAETH_ESW_IGMP_SNOOP_OFF is not set
CONFIG_RAETH_ESW_IGMP_SNOOP_SW=y
CONFIG_RAETH_ESW_PORT_WAN=0
CONFIG_RAETH_ESW_PORT_LAN1=4
CONFIG_RAETH_ESW_PORT_LAN2=2
CONFIG_RAETH_ESW_PORT_LAN3=3
CONFIG_RAETH_ESW_PORT_LAN4=1
```
>- led: >>>> board.h
```shell
#undef  BOARD_GPIO_LED_ALL 
#define BOARD_GPIO_LED_WIFI	11
#define BOARD_GPIO_LED_POWER	24	/* 24: blue, 26: yellow, 29: red */
#undef  BOARD_GPIO_LED_LAN
#undef  BOARD_GPIO_LED_WAN
```

- 小米路由4C 网口以及LED灯配置分别如下
>- wlan and lan: >>>>> kernel-3.4.x.config
```shell
# CONFIG_RAETH_ESW_IGMP_SNOOP_OFF is not set
CONFIG_RAETH_ESW_IGMP_SNOOP_SW=y
CONFIG_RAETH_ESW_PORT_WAN=1
CONFIG_RAETH_ESW_PORT_LAN1=4
CONFIG_RAETH_ESW_PORT_LAN2=2
CONFIG_RAETH_ESW_PORT_LAN3=3
CONFIG_RAETH_ESW_PORT_LAN4=0
```
>- led: >>>> board.h
```shell
#undef  BOARD_GPIO_LED_ALL 
#define BOARD_GPIO_LED_WIFI	11
#define BOARD_GPIO_LED_POWER	24	/* 24: blue, 26: yellow, 29: red */
#undef  BOARD_GPIO_LED_LAN
#undef  BOARD_GPIO_LED_WAN
```
***

### 编译说明 ###

* 安装依赖包
```shell
sudo apt-get update
sudo apt-get install unzip libtool curl cmake gperf gawk flex bison nano \
git python-docutils gettext automake autopoint texinfo build-essential fakeroot \
pkg-config zlib1g-dev libgmp3-dev libmpc-dev libmpfr-dev libncurses5-dev libltdl-dev
```
* 克隆源码
```shell
git clone --depth=1 https://github.com/yuos-bit/Padavan.git /opt/rt-n56u
#git clone --depth=1 https://github.com/yuos-bit/Padavan.git /opt/rt-n56u
```
* 编译工具链
```shell
cd /opt/rt-n56u/toolchain-mipsel
./clean_sources
./build_toolchain_3.4.x
```
* (可选)修改机型配置文件
```shell
nano /opt/rt-n56u/trunk/configs/templates/PSG1218.config
```
* 清理代码树并开始编译
```shell
cd /opt/rt-n56u/trunk
sudo ./clear_tree
fakeroot ./build_firmware_modify PSG1218
#脚本第一个参数为路由型号，在trunk/configs/templates/中
#编译好的固件在trunk/images里
```

***

### 请参阅 ###
- https://yuos.top/index.php/archives/11/
- https://yuos.top/index.php/archives/208/
