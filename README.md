![visitor badge](https://visitor-badge.laobi.icu/badge?page_id=keyword&title=viewers) ![GitHub all releases](https://img.shields.io/github/downloads/stephensund/OpenWrt-AutoBuild/total?style=flat-square)

编译个人自用的设备以及部分热门设备的OpenWrt固件，有需要的朋友请移步actions页面[Github Actions](https://github.com/stephensund/Openwrt-Actions/actions)或Release页面[Releases](https://github.com/stephensund/OpenWrt-AutoBuild/releases)自行下载，同时对应的Workflow页面和Release页面会有**奶牛快传**和**WeTransfer**的下载链接

**个人无偿兴趣项目，不提供任何技术支持，请多动手上网搜寻相关知识，插件等问题请直接向源码维护者反馈，简介后面贴了一些主要插件的仓库地址**

感谢[P3TERX/Actions-Openwrt](https://github.com/P3TERX/Actions-OpenWrt)提供的脚本    
感谢Lean [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)和CTCGFW's Team [project-openwrt/openwrt](https://github.com/project-openwrt/openwrt)

源码均使用[project-openwrt/openwrt](https://github.com/project-openwrt/openwrt) openwrt-18.06-k5.4分支

**已加入update-checker，每天CST 0:00自动检测源码更新，检测到更新后自动触发编译**

默认LAN IP:192.168.2.1

默认用户名root，密码password

## 编译设备
|   设备   |  编译状态  |  对应Actions链接  |
|  ----  |  ----  |  ----  |
|  X86_64  | ![X86_64](https://img.shields.io/github/workflow/status/stephensund/Actions-OpenWrt/X86_64-Openwrt?style=flat-square) |  <a href="https://github.com/stephensund/Actions-OpenWrt/actions?query=workflow%3AX86_64-Openwrt"><img src="https://img.shields.io/badge/Actions-x86__64-blueviolet?style=flat-square" alt="x86_64"></a>  |
|  ASUS RT-ACRH17  | ![ACRH17](https://img.shields.io/github/workflow/status/stephensund/Actions-OpenWrt/ACRH17-Openwrt?style=flat-square) |  <a href="https://github.com/stephensund/Actions-OpenWrt/actions?query=workflow%3AACRH17-Openwrt"><img src="https://img.shields.io/badge/Actions-ACRH17-blueviolet?style=flat-square" alt="ACRH17"></a>  |
|  竞斗云/P&W R619AC  |  ![GDock](https://img.shields.io/github/workflow/status/stephensund/Actions-OpenWrt/GDock-OpenWrt?style=flat-square)  |  <a href="https://github.com/stephensund/Actions-OpenWrt/actions?query=workflow%3AGDock-OpenWrt"><img src="https://img.shields.io/badge/Actions-GDock-blueviolet?style=flat-square" alt="R619AC"></a>  |
|  XIAOMI-AC2100  |  ![AC2100](https://img.shields.io/github/workflow/status/stephensund/Actions-OpenWrt/XIAOMI-AC2100-Openwrt?style=flat-square)  |  <a href="https://github.com/stephensund/Actions-OpenWrt/actions?query=workflow%3AXIAOMI-AC2100-Openwrt"><img src="https://img.shields.io/badge/Actions-AC2100-blueviolet?style=flat-square" alt="AC2100"></a>  |
|  Nanopi-R2S |  ![Nanopi-R2S](https://img.shields.io/github/workflow/status/stephensund/Actions-OpenWrt/Nanopi-R2S-Openwrt?style=flat-square)  |  <a href="https://github.com/stephensund/Actions-OpenWrt/actions?query=workflow%3ANanopi-R2S-Openwrt"><img src="https://img.shields.io/badge/Actions-R2S-blueviolet?style=flat-square" alt="R2S"></a>  |
|  REDMI-AC2100  |  ![RM2100](https://img.shields.io/github/workflow/status/stephensund/Actions-OpenWrt/REDMI-AC2100-Openwrt?style=flat-square)  |  <a href="https://github.com/stephensund/Actions-OpenWrt/actions?query=workflow%3AREDMI-AC2100-Openwrt"><img src="https://img.shields.io/badge/Actions-RM2100-blueviolet?style=flat-square" alt="RM2100"></a>  |
|  Nanopi-R4S  |  ![Nanopi-R4S](https://img.shields.io/github/workflow/status/stephensund/Actions-OpenWrt/Nanopi-R4S-Openwrt?style=flat-square)  |  <a href="https://github.com/stephensund/Actions-OpenWrt/actions?query=workflow%3ANanopi-R4S-Openwrt"><img src="https://img.shields.io/badge/Actions-R4S-blueviolet?style=flat-square" alt="R4S"></a>  |
|  ARMv8通用镜像  |  ![ARMv8](https://img.shields.io/github/workflow/status/stephensund/Actions-OpenWrt/ARMv8-Multiplatform?style=flat-square)  |  <a href="https://github.com/stephensund/Actions-OpenWrt/actions?query=workflow%3AARMv8-Multiplatform"><img src="https://img.shields.io/badge/Actions-ARMv8-blueviolet?style=flat-square" alt="ARMv8"></a>  |

## 主要包含插件列表
固件满足基本的上网/代理需求，暂不过多添加其他功能。

* Luci-app-ssr-plus [fw876/helloworld](https://github.com/fw876/helloworld)

* Luci-app-passwall [xiaorouji/openwrt-passwall](https://github.com/xiaorouji/openwrt-passwall)

* Luci-app-openclash [vernesong/Openclash](https://github.com/vernesong/OpenClash)

* Luci-app-smartdns [pymumu/smartdns](https://github.com/pymumu/smartdns)

* Luci-app-adguardhome及其核心文件 [rufengsuixing/luci-app-adguardhome](https://github.com/rufengsuixing/luci-app-adguardhome) [AdguardTeam/AdGuardHome](https://github.com/AdguardTeam/AdGuardHome)

* Luci-app-unblockmusic

* Luci-app-https-dns-proxy 其可在指定端口上运行指定服务商的DoH DNS服务，可以与代理配合使用

* Luci-theme-argon以及用于主题自定义设置的Luci-app-argon-config [jerrykuku/luci-theme-argon](https://github.com/jerrykuku/luci-theme-argon)
