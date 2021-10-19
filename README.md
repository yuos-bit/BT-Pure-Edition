[![Build Status](https://travis-ci.com/hanwckf/rt-n56u.svg?branch=master)](https://travis-ci.com/hanwckf/rt-n56u)
![GitHub All Releases](https://img.shields.io/github/downloads/hanwckf/rt-n56u/total)
[![release](https://img.shields.io/github/release/hanwckf/rt-n56u.svg)](https://github.com/hanwckf/rt-n56u/releases)

# README #

### UI预览 ###
[![50MtR1.png](https://z3.ax1x.com/2021/10/19/50MtR1.png)](https://imgtu.com/i/50MtR1)

### 宝塔纯净版介绍 ###
* 基于BT官方剥离了所有与BT官方的通信、上报、下发、以及登录绑定手机号才能使用的功能；
* 所有功能与原版一致，不会有任何异常，如有任何问题请参考宝塔官方解决方案；
* 提升为企业会员，软件商店中的所有[运行环境]、[免费插件]、[宝塔插件]、[专业版插件]、[企业版插件]；部分[第三方应用]安装可能会失败。
### 特别说明 ###
* 1.该项目只是收集网上的开源项目用于本地虚拟机测试以及小白建站测试，请不要使用于违法途径
* 2.开源无情人有情，请不要滥用或者出售脚本，让脚本制作的大佬遭受不白之冤
* 3.脚本不一定什么时候就没了，记得及时建立快照

***

### 脚本1 ###
* 来源:https://www.roamacg.com/1193.html

宝塔7.5.1专业版

* 安装要求
内存：512M以上，推荐768M以上（纯面板约占系统60M内存） 硬盘：100M以上可用硬盘空间（纯面板约占20M磁盘空间） 系统：CentOS 7.1+ (Ubuntu16.04+.、Debian9.0+)，确保是干净的操作系统，没有安装过其它环境带的Apache/Nginx/php/MySQL（已有环境不可安装） ### NEW端口：8888

安装脚本
Centos 安裝腳本 面板端口：8888
```shell
yum install -y wget && wget -O install.sh https://download.fenhao.me/install/install_6.0.sh && sh install.sh
```

試驗性 Centos/Ubuntu/Debian 安裝命令 獨立運行環境（py3.7） 可能存在少量兼容性問題 不斷優化中
```shell
curl -sSO https://download.fenhao.me/install/install_panel.sh && bash install_panel.sh
```
Ubuntu/Deepin 安裝腳本
```shell
wget -O install.sh https://download.fenhao.me/install/install-ubuntu_6.0.sh && sudo bash install.sh
```
Debian 安裝腳本
```shell
wget -O install.sh https://download.fenhao.me/install/install-ubuntu_6.0.sh && bash install.sh
```
Fedora 安裝腳本
```shell
wget -O install.sh https://download.fenhao.me/install/install_6.0.sh && bash install.sh
```
Linux 面板 7.5.1 升級命令（已安裝面板或舊版本或免費版升級專業版）
```shell
curl https://download.fenhao.me/install/update6.sh|bash
```
### 脚本来源2 ###
* 来源：https://www.hostcli.com/
宝塔 7.6.0版本 [推荐/稳定版本]

Centos全新安装命令：根据系统执行框内命令开始安装（大约2分钟完成面板安装）升级后可能需要重启面板
```shell
yum install -y wget && wget -O install.sh http://v7.hostcli.com/install/install_6.0.sh && sh install.sh
```
Ubuntu/Deepin全新安装命令：
```shell
wget -O install.sh http://v7.hostcli.com/install/install-ubuntu_6.0.sh && sudo bash install.sh
```

Debian全新安装命令：
```shell
wget -O install.sh http://v7.hostcli.com/install/install-ubuntu_6.0.sh && bash install.sh
```
Fedora全新安装命令:：
```shell
wget -O install.sh http://v7.hostcli.com/install/install_6.0.sh && bash install.sh
```
已经安装官方面板，执行下列命令升级到7.6.0纯净版：
```shell
curl http://v7.hostcli.com/install/update6.sh|bash
```
其他非官方版本(含开心版、快乐版、纯净版等 7.4.5至7.6.0版本之间所有版本均可)，执行下列命令升级到7.6.0纯净版：
```shell
curl http://v7.hostcli.com/install/update6.sh|bash
```
任意非官方版本还原到官方最新版
```shell
curl http://download.bt.cn/install/update6.sh|bash
```
***

### 引用 ###
- https://www.roamacg.com/1193.html
- https://www.hostcli.com/
