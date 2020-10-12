# k3_packages_backup
> k3的固件和插件备份仓库，自己编译自己使用，仅此备份，按需自取。  
> 有时间会解答你们的安装或者编译问题，没时间也请见谅，谢谢。  
> 编译环境为 Ubuntu 18.04 Desktop x64，大雕的说明没有说是桌面版本还是服版本，再次提醒下想自己编译的朋友。  
> 源码来自[lede](https://github.com/coolsnowwolf/lede)，更多问题解答请前往他的`issue`里面搜索下，不要什么不懂，张嘴就问！要培养自己的`problems solving skill`。  
> 如果需要加入一些特殊功能，请在克隆后把`lede`目录下的`feeds.conf.default`文件的`#src-git helloworld https://github.com/fw876/helloworld` `#`去掉然后在按照步骤开始编译

## 备份插件文件列表
### 编译时间:2020/09/01

```other
.
├── brcmfmac-firmware-usb_20200619-1_arm_cortex-a9.ipk
├── busybox_1.31.1-2_arm_cortex-a9.ipk
├── ca-certificates_20200601-1_all.ipk
├── coremark_2020-05-28-7685fd32-15_arm_cortex-a9.ipk
├── ddns-scripts_aliyun_1.0.3-1_all.ipk
├── ddns-scripts_dnspod_1.0.2-1_all.ipk
├── default-settings_2-3_all.ipk
├── dns2socks_2.1-1_arm_cortex-a9.ipk
├── dnsmasq-full_2.81-7_arm_cortex-a9.ipk
├── dropbear_2020.80-1_arm_cortex-a9.ipk
├── firewall_2019-11-22-8174814a-1_arm_cortex-a9.ipk
├── getrandom_2019-12-31-0e34af14-4_arm_cortex-a9.ipk
├── hostapd-common_2020-06-08-5a8b3662-4_arm_cortex-a9.ipk
├── ip-full_5.7.0-2_arm_cortex-a9.ipk
├── ipset_7.4-1_arm_cortex-a9.ipk
├── ipt2socks_1.1.3-1_arm_cortex-a9.ipk
├── iptables-mod-fullconenat_2019-10-21-0cf3b48f-3_arm_cortex-a9.ipk
├── iw_5.4-1_arm_cortex-a9.ipk
├── jshn_2020-05-25-66195aee-1_arm_cortex-a9.ipk
├── jsonfilter_2018-02-04-c7e938d6-1_arm_cortex-a9.ipk
├── k3screenctrl_0.10-2_arm_cortex-a9.ipk
├── k3wifi_1-2_arm_cortex-a9.ipk
├── libblobmsg-json_2020-05-25-66195aee-1_arm_cortex-a9.ipk
├── libelf1_0.179-1_arm_cortex-a9.ipk
├── libevent2-7_2.1.11-2_arm_cortex-a9.ipk
├── libipset13_7.4-1_arm_cortex-a9.ipk
├── libjson-c4_0.13.1-2_arm_cortex-a9.ipk
├── libjson-script_2020-05-25-66195aee-1_arm_cortex-a9.ipk
├── liblua5.1.5_5.1.5-7_arm_cortex-a9.ipk
├── libmbedtls12_2.16.7-1_arm_cortex-a9.ipk
├── libmnl0_1.0.4-2_arm_cortex-a9.ipk
├── libnl-tiny_2019-10-29-0219008c-1_arm_cortex-a9.ipk
├── libopenssl1.1_1.1.1g-1_arm_cortex-a9.ipk
├── libopenssl-conf_1.1.1g-1_arm_cortex-a9.ipk
├── libpcre_8.44-2_arm_cortex-a9.ipk
├── libubox20191228_2020-05-25-66195aee-1_arm_cortex-a9.ipk
├── libubus20191227_2020-02-05-171469e3-1_arm_cortex-a9.ipk
├── libubus-lua_2020-02-05-171469e3-1_arm_cortex-a9.ipk
├── libuci_2018-08-11-4c8b4d6e-2_arm_cortex-a9.ipk
├── libuci-lua_2018-08-11-4c8b4d6e-2_arm_cortex-a9.ipk
├── libuclient20160123_2020-06-17-c6609861-1_arm_cortex-a9.ipk
├── libustream-openssl20200215_2020-03-13-5e1bc342-1_arm_cortex-a9.ipk
├── libuuid1_2.35.1-2_arm_cortex-a9.ipk
├── logd_2019-12-31-0e34af14-4_arm_cortex-a9.ipk
├── lua_5.1.5-7_arm_cortex-a9.ipk
├── luci-app-accesscontrol_1-11_all.ipk
├── luci-app-arpbind_1-3_all.ipk
├── luci-app-autoreboot_1.0-8_all.ipk
├── luci-app-cpufreq_1-5_all.ipk
├── luci-app-filetransfer_1-2_all.ipk
├── luci-app-ramfree_1.0-1_all.ipk
├── luci-app-sfe_1.0-13_all.ipk
├── luci-app-ttyd_1.0-3_all.ipk
├── luci-app-unblockmusic_2.3.5-9_all.ipk
├── luci-app-vlmcsd_1.0-5_all.ipk
├── luci-app-vsftpd_1.0-3_all.ipk
├── luci-app-webadmin_2-1_all.ipk
├── luci-i18n-accesscontrol-zh-cn_1-11_all.ipk
├── luci-i18n-arpbind-zh-cn_1-3_all.ipk
├── luci-i18n-autoreboot-zh-cn_1.0-8_all.ipk
├── luci-i18n-cpufreq-zh-cn_1-5_all.ipk
├── luci-i18n-filetransfer-zh-cn_1-2_all.ipk
├── luci-i18n-ramfree-zh-cn_1.0-1_all.ipk
├── luci-i18n-sfe-zh-cn_1.0-13_all.ipk
├── luci-i18n-ttyd-zh-cn_1.0-3_all.ipk
├── luci-i18n-unblockmusic-zh-cn_2.3.5-9_all.ipk
├── luci-i18n-vlmcsd-zh-cn_1.0-5_all.ipk
├── luci-i18n-vsftpd-zh-cn_1.0-3_all.ipk
├── luci-i18n-webadmin-zh-cn_2-1_all.ipk
├── luci-lib-fs_1.0-1_all.ipk
├── microsocks_1.0-1_arm_cortex-a9.ipk
├── netifd_2020-06-06-51e9fb81-1_arm_cortex-a9.ipk
├── openssl-util_1.1.1g-1_arm_cortex-a9.ipk
├── openwrt-keyring_2019-07-25-8080ef34-1_arm_cortex-a9.ipk
├── opkg_2020-05-07-f2166a89-1_arm_cortex-a9.ipk
├── Packages
├── Packages.gz
├── Packages.manifest
├── Packages.sig
├── pdnsd-alt_1.2.9b-par-a8e46ccba7b0fa2230d6c42ab6dcd92926f6c21d_arm_cortex-a9.ipk
├── ppp_2.4.8-5_arm_cortex-a9.ipk
├── ppp-mod-pppoe_2.4.8-5_arm_cortex-a9.ipk
├── procd_2020-05-28-b9b39e20-2_arm_cortex-a9.ipk
├── redsocks2_0.67-4_arm_cortex-a9.ipk
├── resolveip_2_arm_cortex-a9.ipk
├── rpcd_2020-05-26-078bb57e-1_arm_cortex-a9.ipk
├── shadowsocksr-libev-alt_2.5.6-5_arm_cortex-a9.ipk
├── shadowsocksr-libev-server_2.5.6-5_arm_cortex-a9.ipk
├── shadowsocksr-libev-ssr-local_2.5.6-5_arm_cortex-a9.ipk
├── shellsync_0.2-2_arm_cortex-a9.ipk
├── simple-obfs_0.0.5-5_arm_cortex-a9.ipk
├── swconfig_12_arm_cortex-a9.ipk
├── trojan_1.16.0-1_arm_cortex-a9.ipk
├── ubox_2019-12-31-0e34af14-4_arm_cortex-a9.ipk
├── ubus_2020-02-05-171469e3-1_arm_cortex-a9.ipk
├── ubusd_2020-02-05-171469e3-1_arm_cortex-a9.ipk
├── uci_2018-08-11-4c8b4d6e-2_arm_cortex-a9.ipk
├── uclient-fetch_2020-06-17-c6609861-1_arm_cortex-a9.ipk
├── uhttpd_2020-06-03-939c281c-2_arm_cortex-a9.ipk
├── uhttpd-mod-ubus_2020-06-03-939c281c-2_arm_cortex-a9.ipk
├── UnblockNeteaseMusicGo_0.2.4-1_arm_cortex-a9.ipk
├── urandom-seed_1.0-2_arm_cortex-a9.ipk
├── urngd_2020-01-21-c7f7b6b6-1_arm_cortex-a9.ipk
├── usign_2020-05-23-f1f65026-1_arm_cortex-a9.ipk
├── v2ray_4.31.0-1_arm_cortex-a9.ipk
├── v2ray-plugin_1.4.1-1_arm_cortex-a9.ipk
├── vlmcsd_svn1113-1_arm_cortex-a9.ipk
├── vsftpd-alt_3.0.3-7_arm_cortex-a9.ipk
├── wget_1.20.3-4_arm_cortex-a9.ipk
├── wireless-regdb_2020.04.29-1_all.ipk
├── wol_0.7.1-3_arm_cortex-a9.ipk
├── wpad-basic_2020-06-08-5a8b3662-4_arm_cortex-a9.ipk
└── zlib_1.2.11-3_arm_cortex-a9.ipk

0 directories, 113 files


```
