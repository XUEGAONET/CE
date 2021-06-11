# clearWrt

## Intro. 

**based on OpenWrt 19.07 branch**

A customized opearting system based on openwrt for special needs such as the section below. This repository stays in sync with the upstream and can release the newest version by GitHub Action automatically. So, you can get the newest stable firmware in here. :relaxed:

**For more details, you can visit http://www.openwrt.org.**

## Usage

:arrow_right: You can visit **[here](https://github.com/XUEGAONET/clearWrt/releases/latest)** to download latest released firmware for installation or upgradation.

## Differences

* Security
  * RELRO enabled
  * Aggressive buffer-overflow detection enabled
  * GCC fotmat-security enabled
  * Userspace ASLR PIE compilation enabled
  * PIE enabled by default
  * Stack-Smashing Protection enabled by default
* Stability
  * Soft and hard lockup panic enabled
  * Auto reboot after panic
* Routing
  * Full featured FRRouting intergrated
* Monitoring
  * Zabbix agent intergrated



