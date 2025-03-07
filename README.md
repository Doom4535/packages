fantastic packages
==================

[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fantastic-packages/packages/AutoBuild.yml?label=AutoBuild&style=flat-square)](https://github.com/fantastic-packages/packages/actions/workflows/AutoBuild.yml)
[![Website](https://img.shields.io/website?down_message=offline&label=Donwload%20pages&style=flat-square&up_message=online&url=https%3A%2F%2Ffantastic-packages.github.io%2Fpackages%2F)](https://fantastic-packages.github.io/packages/)
[![Website](https://img.shields.io/website?down_message=userguide&label=Custom%20Feeds&style=flat-square&up_message=userguide&url=https%3A%2F%2Fgithub.com%2Ffantastic-packages%2Fpackages%2Ftree%2Fgh-pages)](https://github.com/fantastic-packages/packages/tree/gh-pages#how-to-use-on-openwrt)
[![GitHub](https://img.shields.io/github/license/fantastic-packages/packages?style=flat-square)](./LICENSE)

### How to use

1. Add to `feeds.conf.default`
```shell
umask 022
sed -i '1i src-git fantastic-packages https://github.com/fantastic-packages/packages' feeds.conf.default
./scripts/feeds update -a
./scripts/feeds install -a
make menuconfig
```

2. Pull in the src/sdk directory
```shell
umask 022
git clone --depth 1 --branch master --single-branch --no-tags --recurse-submodules https://github.com/fantastic-packages/packages package/fantastic-packages
make menuconfig
```

### Package description
| Packages | Description |
| ---- | ---- |
| [luci-app-alwaysonline][] | Hijack/bypass Windows NCSI and iOS portal detection |
| [luci-app-change-mac][] | MAC address randomizer for LuCI |
| [luci-app-cpu-perf][] | CPU performance information and management for LuCI |
| [luci-app-cpu-status][] | CPU utilization info for the LuCI status page |
| [luci-app-cpu-status-mini][] | CPU utilization info for the LuCI status page |
| [luci-app-diskman][] | A Simple Disk Manager for LuCI |
| [luci-app-disks-info][] | Information about connected disk devices (partitions, filesystems, SMART) for LuCI |
| [luci-app-dnsproxy][] | A simple DNS proxy server |
| [luci-app-interfaces-statistics][] | Network interfaces statistics for LuCI |
| [luci-app-internet-detector][] | Internet detector for OpenWrt |
| [luci-app-log][] | Advanced syslog and kernel log (tail, search, etc) for LuCI |
| [luci-app-natmapt][] | TCP/UDP port mapping for LuCI |
| [luci-app-natter][] | TCP/UDP hole punching tool for LuCI |
| [luci-app-netdata][] | Netdata for LuCI |
| [luci-app-netspeedtest][] | Network Speed Test LuCI |
| [luci-app-packagesync][] | Used to build a local mirror feeds source on the router |
| [luci-app-pcap-dnsproxy][] | A DNS server for LuCI |
| [luci-app-serverchan][] | Service push |
| [luci-app-temp-status][] | Temperature sensors data for the LuCI status page |
| [luci-app-tinyfilemanager][] | Web based File Manager in PHP |
| [luci-app-tn-netports][] | Network ports status LuCI |
| [luci-theme-argon][] | A clean and tidy OpenWrt LuCI theme |
| [luci-app-argon-config][] | Argon Theme Config Plugin |
| [openwrt-alwaysonline][] | Hijack/bypass Windows NCSI and iOS portal detection |
| [openwrt-chinadns-ng][] | ChinaDNS Next Generation for OpenWrt, refactoring with epoll and ipset |
| [openwrt-go-stun][] | A GO STUN client |
| [openwrt-natmapt][] | TCP/UDP port mapping for full cone NAT |
| [openwrt-Natter][] | TCP/UDP hole punching tool |
| [openwrt-netdata-ssl][] | Real-time performance monitoring tool |
| [openwrt-Pcap_DNSProxy][] | Pcap_DNSProxy for OpenWrt/LEDE |
| [openwrt-php-nginx][] | PHP with Nginx as Webserver |
| [openwrt-rgmac][] | a simple random MAC address generator for OpenWRT |
| [openwrt-stuntman][] | an open source STUN server and client code by john selbie |
| [openwrt-Toolkit][] | DNS Toolkit |

--------

[luci-app-alwaysonline]: https://github.com/muink/luci-app-alwaysonline
[luci-app-change-mac]: https://github.com/muink/luci-app-change-mac
[luci-app-cpu-perf]: https://github.com/gSpotx2f/luci-app-cpu-perf
[luci-app-cpu-status]: https://github.com/gSpotx2f/luci-app-cpu-status
[luci-app-cpu-status-mini]: https://github.com/gSpotx2f/luci-app-cpu-status-mini
[luci-app-diskman]: https://github.com/lisaac/luci-app-diskman
[luci-app-disks-info]: https://github.com/gSpotx2f/luci-app-disks-info
[luci-app-dnsproxy]: https://github.com/muink/luci-app-dnsproxy
[luci-app-interfaces-statistics]: https://github.com/gSpotx2f/luci-app-interfaces-statistics
[luci-app-internet-detector]: https://github.com/gSpotx2f/luci-app-internet-detector
[luci-app-log]: https://github.com/gSpotx2f/luci-app-log
[luci-app-natmapt]: https://github.com/muink/luci-app-natmapt
[luci-app-natter]: https://github.com/muink/luci-app-natter
[luci-app-netdata]: https://github.com/muink/luci-app-netdata
[luci-app-netspeedtest]: https://github.com/muink/luci-app-netspeedtest
[luci-app-packagesync]: https://github.com/muink/luci-app-packagesync
[luci-app-pcap-dnsproxy]: https://github.com/muink/luci-app-pcap-dnsproxy
[luci-app-serverchan]: https://github.com/tty228/luci-app-wechatpush
[luci-app-temp-status]: https://github.com/gSpotx2f/luci-app-temp-status
[luci-app-tinyfilemanager]: https://github.com/muink/luci-app-tinyfilemanager
[luci-app-tn-netports]: https://github.com/muink/luci-app-tn-netports
[luci-theme-argon]: https://github.com/jerrykuku/luci-theme-argon
[luci-app-argon-config]: https://github.com/jerrykuku/luci-app-argon-config
[openwrt-alwaysonline]: https://github.com/muink/openwrt-alwaysonline
[openwrt-chinadns-ng]: https://github.com/muink/openwrt-chinadns-ng
[openwrt-go-stun]: https://github.com/muink/openwrt-go-stun
[openwrt-natmapt]: https://github.com/muink/openwrt-natmapt
[openwrt-Natter]: https://github.com/muink/openwrt-Natter
[openwrt-netdata-ssl]: https://github.com/muink/openwrt-netdata-ssl
[openwrt-Pcap_DNSProxy]: https://github.com/muink/openwrt-Pcap_DNSProxy
[openwrt-php-nginx]: https://github.com/muink/openwrt-php-nginx
[openwrt-rgmac]: https://github.com/muink/openwrt-rgmac
[openwrt-stuntman]: https://github.com/muink/openwrt-stuntman
[openwrt-Toolkit]: https://github.com/muink/openwrt-Toolkit
