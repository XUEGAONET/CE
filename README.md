# clearWrt

## Intro. 

**based on OpenWrt 19.07 branch**

A customized opearting system based on openwrt for special needs such as the section below. This repository stays in sync with the upstream and can release the newest version by GitHub Action automatically. So, you can get the newest stable firmware in here. :relaxed:

**For more details, you can visit http://www.openwrt.org.**

## Usage

:arrow_right: You can visit **[here](https://github.com/XUEGAONET/clearWrt/releases)** to download the released firmware you need for installation or upgradation.

Please pay attention to the field named `Config Name` which also can be construed as `Profile`. Different `Config Name` will lead to firmware for different usage.

## Differences

* Security
  * ~~RELRO enabled~~ deprecated because of effect on performance
  * ~~Aggressive buffer-overflow detection enabled~~ deprecated because of effect on performance
  * ~~GCC format-security enabled~~ deprecated because of effect on performance
  * ~~Userspace ASLR PIE compilation enabled~~ deprecated because of effect on performance
  * ~~PIE enabled by default~~ deprecated because of effect on performance
  * ~~Stack-Smashing Protection enabled by default~~ deprecated because of effect on performance
* Stability
  * Soft and hard lockup panic enabled
  * Auto reboot after panic
* Routing
  * Full featured FRRouting intergrated
* Monitoring
  * Zabbix agent intergrated



