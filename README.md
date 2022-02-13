[![Build Status](https://travis-ci.com/hanwckf/rt-n56u.svg?branch=master)](https://travis-ci.com/hanwckf/rt-n56u)
![GitHub All Releases](https://img.shields.io/github/downloads/hanwckf/rt-n56u/total)
[![release](https://img.shields.io/github/release/hanwckf/rt-n56u.svg)](https://github.com/hanwckf/rt-n56u/releases)

# README #

### UI预览 ###
[![5014eK.png](https://z3.ax1x.com/2021/10/19/5014eK.png)](https://imgtu.com/i/5014eK)
[![501fL6.png](https://z3.ax1x.com/2021/10/19/501fL6.png)](https://imgtu.com/i/501fL6)
[![50MtR1.png](https://z3.ax1x.com/2021/10/19/50MtR1.png)](https://imgtu.com/i/50MtR1)

### 宝塔纯净版介绍 ###
* 基于BT官方剥离了所有与BT官方的通信、上报、下发、以及登录绑定手机号才能使用的功能；
* 所有功能与原版一致，不会有任何异常，如有任何问题请参考宝塔官方解决方案；
* 提升为企业会员，软件商店中的所有[运行环境]、[免费插件]、[宝塔插件]、[专业版插件]、[企业版插件]；部分[第三方应用]安装可能会失败。
### 特别说明 ###
* 1.该项目只是收集网上的开源项目用于本地虚拟机测试以及小白建站测试，请不要使用于违法途径
* 2.开源无情人有情，请不要滥用或者出售脚本，让脚本制作的大佬遭受不白之冤
* 3.脚本不一定什么时候就没了，记得及时建立快照
* 4.emmmm，至于后门问题，大佬说是没有的，但是你要用那么后果你自己承担，懂？周瑜打黄盖，不要出问题后来逼逼赖赖！

***

### 脚本1 ###
* 来源:https://www.roamacg.com/1271.html

专业版：

Centos安装命令：
```
yum install -y wget && wget -O install.sh http://download.moetas.com/install/install_6.0.sh && sh install.sh
```
试验性Centos/Ubuntu/Debian安装命令 独立运行环境（py3.7） 可能存在少量兼容性问题 不断优化中
```
curl -sSO http://download.moetas.com/install/install_panel.sh && bash install_panel.sh
```
Ubuntu Deepin安装命令：
```
wget -O install.sh http://download.moetas.com/install/install-ubuntu_6.0.sh && sudo bash install.sh
```
Debian安装命令：
```
wget -O install.sh http://download.moetas.com/install/install-ubuntu_6.0.sh && bash install.sh
```
Fedora安装命令:
```
wget -O install.sh http://download.moetas.com/install/install_6.0.sh && bash install.sh
```
Linux面板7.7.0升级专业版命令：
```
curl http://download.moetas.com/install/update6.sh|bash
```
企业版：
Centos安装命令：
```
yum install -y wget && wget -O install.sh http://download.moetas.com/ltd/install/install_6.0.sh && sh install.sh
```
试验性Centos/Ubuntu/Debian安装命令 独立运行环境（py3.7） 可能存在少量兼容性问题 不断优化中
```
curl -sSO http://download.moetas.com/ltd/install/install_panel.sh && bash install_panel.sh
```
Ubuntu Deepin安装命令：
```
wget -O install.sh http://download.moetas.com/ltd/install/install-ubuntu_6.0.sh && sudo bash install.sh
```
Debian安装命令：
```
wget -O install.sh http://download.moetas.com/ltd/install/install-ubuntu_6.0.sh && bash install.sh
```
Fedora安装命令:
```
wget -O install.sh http://download.moetas.com/ltd/install/install_6.0.sh && bash install.sh
```
Linux面板7.7.0升级企业版命令：
```
curl http://download.moetas.com/ltd/install/update6.sh|bash
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
