[![Build Status](https://travis-ci.com/hanwckf/rt-n56u.svg?branch=master)](https://travis-ci.com/hanwckf/rt-n56u)
![GitHub All Releases](https://img.shields.io/github/downloads/hanwckf/rt-n56u/total)
[![release](https://img.shields.io/github/release/hanwckf/rt-n56u.svg)](https://github.com/hanwckf/rt-n56u/releases)

# README #

### UI预览

[![5014eK.png](https://z3.ax1x.com/2021/10/19/5014eK.png)](https://imgtu.com/i/5014eK)
[![501fL6.png](https://z3.ax1x.com/2021/10/19/501fL6.png)](https://imgtu.com/i/501fL6)
[![50MtR1.png](https://z3.ax1x.com/2021/10/19/50MtR1.png)](https://imgtu.com/i/50MtR1)

### 宝塔纯净版介绍

* 基于BT官方剥离了所有与BT官方的通信、上报、下发、以及登录绑定手机号才能使用的功能；
* 所有功能与原版一致，不会有任何异常，如有任何问题请参考宝塔官方解决方案；
* 提升为企业会员，软件商店中的所有[运行环境]、[免费插件]、[宝塔插件]、[专业版插件]、[企业版插件]；部分[第三方应用]安装可能会失败。

### 特别说明

* 1.该项目只是收集网上的开源项目用于本地虚拟机测试以及小白建站测试，请不要使用于违法途径
* 2.开源无情人有情，请不要滥用或者出售脚本，让脚本制作的大佬遭受不白之冤
* 3.脚本不一定什么时候就没了，记得及时建立快照
* 4.emmmm，至于后门问题，大佬说是没有的，但是你要用那么后果你自己承担，懂？周瑜打黄盖，不要出问题后来逼逼赖赖！

***

### 脚本1

* 来源:[https://www.roamacg.com/1271.html](http://www.btkaixin.net/)

Linux 宝塔面板11.5.0安装脚本：

```shell
if [ -f /usr/bin/curl ];then curl -sSO https://bt11.bthappy.com/install/install_panel.sh;else wget -O install_panel.sh https://bt11.bthappy.com/install/install_panel.sh;fi;bash install_panel.sh bt11.bthappy.com
```
宝塔云安全监控2.3.2安装脚本:
```shell
if [ -f /usr/bin/curl ];then curl -sSO https://bt11.bthappy.com/install/install_btmonitor.sh;else wget -O install_btmonitor.sh https://bt11.bthappy.com/install/install_btmonitor.sh;fi;bash install_btmonitor.sh bt11.bthappy.com
```

### 脚本2

* 来源：<https://www.hostcli.com/>
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

### 脚本3

* 来源:[https://github.com/Closty/happpyBT](https://github.com/Closty/happpyBT)

5合1 安装命令（宝塔 7.0.2 开心版面板）：Ubuntu/Debian需安装`apt-get install wget apt-get install` e2fsprogs

```
yum -y install wget && yum -y install e2fsprogs && wget https://52bt.cn/install/diyu.sh && bash diyu.sh
```

Bt_Panel_Pro 腳本（Centos）：极速安装方式 (安装时间1至10分钟)

```
yum -y install wget;wget https://52bt.cn/install/install_6.0.sh && bash install_6.0.sh
```

Bt_Panel_Pro 腳本（Centos/Ubuntu/Debian支持ipv6）：极速安装方式 (安装时间1至10分钟)

```
curl -sSO https://52bt.cn/install/new_install.sh && bash new_install.sh
```

Bt_Panel_Pro 腳本（Ubuntu）：极速安装方式 (安装时间1至10分钟)

```
wget -O install.sh https://52bt.cn/install/install-ubuntu_6.0.sh && sudo bash install.sh
```

Bt_Panel_Pro 腳本（Debian）：极速安装方式 (安装时间1至10分钟)

```
wget -O install.sh https://52bt.cn/install/install-ubuntu_6.0.sh && bash install.sh
```

Bt_Panel_Pro 腳本（Fedora）：极速安装方式 (安装时间1至10分钟)

```
wget -O install.sh https://52bt.cn/install/install_6.0.sh && bash install.sh
```

已经安装面板
Bt_Panel 脚本（升级开心版）：极速安装方式 (安装时间1至10秒)

```
curl https://52bt.cn/install/update6.sh|bash
```

Nginx防火墙脚本
Bt_Panel 防火墙脚本（一定要安装好Nginx环境）：
防火墙需要面板先安装，然后在使用脚本安装防火墙，请勿在面板升级防火墙！（请勿面板私自升级防火墙，否则无法使用！）

```
wget https://52bt.cn/install/btwaf.sh && bash btwaf.sh
```

Apache防火墙脚本
注意：防火墙需要面板先安装，然后在使用脚本安装防火墙，请勿在面板升级防火墙！（请勿面板私自升级防火墙，否则无法使用！）
注意：该版本是书记之前发布的最后一个版本，虽然很老旧，但是依然可以使用，欢迎大家提供Apache 7.2 - 6.9版本防火墙的文件！

```
wget https://52bt.cn/install/btwaf_httpd.sh && bash btwaf_httpd.sh
```

宝塔同步工具
安装此插件打开可能会报错，需要重启面板就可以正常使用！
第三方插件免费脚本

```
wget -O plugin3.sh https://52bt.cn/install/plugin3.sh && bash plugin3.sh
```

不想使用開心版的，直接使用官方腳本轉成免費

```
wget -O update.sh http://download.bt.cn/install/update.sh && bash update.sh free
```

### 引用 ###

- <https://www.roamacg.com/1193.html>
* <https://www.hostcli.com/>
