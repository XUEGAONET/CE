# clearWrt

## Intro. 

**based on OpenWrt 19.07 stable branch**

A customized opearting system based on openwrt for special needs such as the section below. This repository stays in sync with the upstream and can release the newest version by GitHub Action automatically. So, you can get the newest stable firmware in here. :relaxed:

**For more details, you can visit http://www.openwrt.org.**

## With clearWrt, you can...
* Support youself's SD-WAN customer edge
* Support BGP and ECMP cheaply in anywhere
* Support interface mangment, checking and auto-fix, powered by ifman
## Support Device

* x86_64
* PW R619AC, LTS only

## Version Management

After August 30, 2021, all commits will be submitted to the branch with **main-** prefix. Then it will be mark as pre-release and have a long time testing in pre-production. In the end, it will merge or rebase to the **main** branch for the production and update from pre-release to release. The stable release will be released in **main** branch, and the long-term version will be released in these branch with **main-** prefix. 

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
  * Full featured [FRRouting](https://frrouting.org/) intergrated
  * Latest [ifman](https://github.com/XUEGAONET/ifman) intergrated
* Monitoring
  * Zabbix agent intergrated
