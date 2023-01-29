# Wifi Pineapple Cloner: Builds

For a long time I have noticed that there are people stealing the authorship of this project that started in 2018.<br>
Also there is people who go further and are selling the devices ready to use...<br>

So to prevent anyone from being scammed paying for something that is public and free, I decided to make a second repo with the builds already generated.


## Issues and Pull Request

All this will be handled in the [original project](https://github.com/xchwarze/wifi-pineapple-cloner).


## Supported devices

All builds are made with:
* OpenWrt 19.07.7
* Wifi Pineapple Cloner (WPC) v3 
* The config used to build was the "universal" (flavor: universal). This is designed to be able to mount a TETRA on any hardware.
<br>

The process will work correctly only if you follow these steps:
* First install OpenWrt 19.07.7 on the device.
* Then install the update you will find in this repository. You must install it with the `do not save configuration over reflash` option checked.
* Your hardware has to have at least 2 wifis and it would be recommended to have 3. To comply with this you can use the usb adapters mentioned in the `recommended setup`.
* Your hardware must have a pendrive or sd card in order to have the available space needed by the pineapple. It has to be formatted using the tool provided by the panel under `Advanced > USB & Storage > Format SD Card`.
* As tetra is made to be used on hardware with 32 MB of flash I had to cut some dependencies from the default installation.<br>
These dependencies will be installed automatically when the pinapple is connected to the internet and booting.<br>
If you want to manually run this process `service complete-setup missing_packages`<br>
Without these dependencies you will not be able to use the live scan type and some modules. However, you will be able to use the timed scans and the rest of the tools.
* The default ssh password is `root`. This will be useful when debugging problems that may occur during installation.
<br>


### MIPS

Brand | Device | Type | CPU (MHz) | Flash (MB) | RAM (MB) | Download |
-------------|-------------|-----------|-----------|-----------|-----------|-----------|
ALFA Network | R36A  | WiFi Router | 650 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/r36a-universal-sysupgrade.bin)
ALFA Network | Hornet-UB x2  | Travel Router | 400 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/hornet-ub-x2-universal-sysupgrade.bin)
Buffalo | WZR-HP-G300NH v1 | WiFi Router | 400 | 32 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wzr-hp-g300nh-universal-sysupgrade.bin)
Buffalo | WZR-HP-AG300H v1 | WiFi Router | 680 | 32 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wzr-hp-ag300h-universal-sysupgrade.bin)
Buffalo | WZR-600DHP  | WiFi Router | 680 | 32 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wzr-600dhp-universal-sysupgrade.bin)
Buffalo | WZR-HP-G300NH2 | WiFi Router | 400 | 32 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wzr-hp-g300nh2-universal-sysupgrade.bin)
Buffalo | WZR-HP-G302H A1A0 | WiFi Router | 400 | 32 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/buffalo_wzr-hp-g302h-a1a0-universal-sysupgrade.bin)
Buffalo | WZR-HP-G450H v1 | WiFi Router | 400 | 32 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wzr-hp-g450h-universal-sysupgrade.bin)
D-Link | DGL-5500 A1 | WiFi Router | 720 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dgl-5500-a1-universal-sysupgrade.bin)
D-Link | DHP-1565  | WiFi Router | 560 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dhp-1565-a1-universal-sysupgrade.bin)
D-Link | DIR-825 C1 | WiFi Router | 560 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dir-825-c1-universal-sysupgrade.bin)
D-Link | DIR-835 A1 | WiFi Router | 560 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dir-835-a1-universal-sysupgrade.bin)
GL.iNet | GL-X750 (Spitz)  | WiFi Router | 650 | 16,microSDXC | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/glinet_gl-x750-universal-sysupgrade.bin)
GL.iNet | GL-MiFi  | Travel Router | 400 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-mifi-universal-sysupgrade.bin)
GL.iNet | GL-AR150  | Travel Router | 400 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-ar150-universal-sysupgrade.bin)
GL.iNet | GL-AR300 v3 | WiFi Router | 560 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-ar300-universal-sysupgrade.bin)
GL.iNet | GL-AR300M-Lite v1 | Travel Router | 650 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/glinet_gl-ar300m-lite-universal-sysupgrade.bin)
GL.iNet | GL-AR300M v1.4.0 | WiFi Router | 650 | 16,128NAND | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-ar300m-universal-sysupgrade.bin)
GL.iNet | GL-AR750  | Travel Router | 650 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-ar750-universal-sysupgrade.bin)
GL.iNet | GL-AR750S v1 | Travel Router | 775 | 16,128NAND,microSDXC | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-ar750s-universal-sysupgrade.bin)
NETGEAR | WNDR3800  | WiFi Router | 680 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wndr3800-universal-sysupgrade.bin)
NETGEAR | WNDR3700 v4 | WiFi Router | 560 | 128NAND | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wndr3700v4-universal-sysupgrade.tar)
NETGEAR | WNDR4300 v1 | WiFi Router | 560 | 128NAND | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wndr4300-universal-sysupgrade.tar)
NETGEAR | WNDR3700 v2 | WiFi Router | 680 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wndr3700v2-universal-sysupgrade.bin)
NETGEAR | WNDRMAC v2 | WiFi Router | 680 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wndrmacv2-universal-sysupgrade.bin)
NETGEAR | WNDRMAC v1 | WiFi Router | 680 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wndrmac-universal-sysupgrade.bin)
TP-Link | Archer A7 v5 | WiFi Router | 750 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/tplink_archer-a7-v5-universal-sysupgrade.bin)
TP-Link | Archer C5 AC1200 v1 | WiFi Router | 720 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/archer-c5-v1-universal-sysupgrade.bin)
TP-Link | Archer C7 v2 - v2.1 | WiFi Router | 720 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/archer-c7-v2-universal-sysupgrade.bin)
TP-Link | Archer C7 v4 | WiFi Router | 775 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/archer-c7-v4-universal-sysupgrade.bin)
TP-Link | Archer C7 v5 | WiFi Router | 750 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/archer-c7-v5-universal-sysupgrade.bin)
TP-Link | Archer C59 v1 | WiFi Router | 775 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/archer-c59-v1-universal-sysupgrade.bin)
TP-Link | Archer C59 v2 | WiFi Router | 775 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/archer-c59-v2-universal-sysupgrade.bin)
TP-Link | TL-WR842N v3 | WiFi Router | 650 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/tl-wr842n-v3-universal-sysupgrade.bin)
TP-Link | TL-WR942N v1 | WiFi Router | 775 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/tl-wr942n-v1-universal-sysupgrade.bin)
TP-Link | TL-WR1043ND v4 | WiFi Router | 750 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/tl-wr1043nd-v4-universal-sysupgrade.bin)
TP-Link | VR200  | WiFi Router | 500 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/tplink_vr200-universal-sysupgrade.bin)
TP-Link | VR200v  | WiFi Router | 500 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/tplink_vr200v-universal-sysupgrade.bin)
ZBT | ZBT-WD323  | WiFi Router | 560 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbtlink_zbt-wd323-universal-sysupgrade.bin)
ZyXEL | NBG6616 A00 | WiFi Router | 720 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/NBG6616-universal-sysupgrade.bin)
ZyXEL | NBG6716 A01 | WiFi Router | 720 | 16,256 | 256 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/nbg6716-universal-sysupgrade.tar)
<br>


### MIPSEL

Brand | Device | Type | CPU (MHz) | Flash (MB) | RAM (MB) | Download |
-------------|-------------|-----------|-----------|-----------|-----------|-----------|
ALFA Network | AC1200RM  | WiFi Router | 580 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/alfa-network_ac1200rm-universal-sysupgrade.bin)
ASUS | RT-AC51U  | WiFi Router | 580 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/rt-ac51u-universal-sysupgrade.bin)
ASUS | RT-AC57U v1 | WiFi Router | 880 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/asus_rt-ac57u-universal-sysupgrade.bin)
D-Link | DIR-510L A1 | Travel Router | 580 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dlink_dir-510l-universal-sysupgrade.bin)
D-Link | DIR-860L B1 | WiFi Router | 880 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dir-860l-b1-universal-sysupgrade.bin)
D-Link | DWR-118 A1 | WiFi Router | 580 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dlink_dwr-118-a1-universal-sysupgrade.bin)
D-Link | DWR-118 A2 | WiFi Router | 580 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dlink_dwr-118-a2-universal-sysupgrade.bin)
D-Link | DWR-922 E2 | WiFi Router | 580 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/dlink_dwr-922-e2-universal-sysupgrade.bin)
GL.iNet | GL-MT300A v1.3 | Travel Router | 580 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-mt300a-universal-sysupgrade.bin)
GL.iNet | GL-MT300N v1 | Travel Router | 580 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-mt300n-universal-sysupgrade.bin)
GL.iNet | GL-MT300N v2 | WiFi Router | 580 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-mt300n-v2-universal-sysupgrade.bin)
GL.iNet | GL-MT750  | WiFi Router | 580 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/gl-mt750-universal-sysupgrade.bin)
NETGEAR | WNDR3700 v5 | WiFi Router | 880 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/wndr3700v5-universal-sysupgrade.bin)
NETGEAR | R6120  | WiFi Router | 580 | 16 | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/netgear_r6120-universal-sysupgrade.bin)
NETGEAR | R6220  | WiFi Router | 880 | 128NAND | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/r6220-universal-sysupgrade.bin)
NETGEAR | R6350  | WiFi Router | 880 | 128NAND | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/netgear_r6350-universal-sysupgrade.bin)
Xiaomi | Mi Router 3 Pro  | WiFi Router | 880 | 256NAND | 512 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/xiaomi_mir3p-universal-sysupgrade.bin)
Xiaomi | Mi WiFi Mini v1 | WiFi Router | 580 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/miwifi-mini-universal-sysupgrade.bin)
Xiaomi | MiWiFi 3G v1 | WiFi Router | 880 | 128NAND | 256 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/xiaomi_mir3g-universal-sysupgrade.bin)
ZBT | WE826-E  | WiFi Router | 580 | 32 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbtlink_zbt-we826-e-universal-sysupgrade.bin)
ZBT | WE826 B0 16M | WiFi Router | 580 | 16,SD | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbt-we826-16M-universal-sysupgrade.bin)
ZBT | WE826 B0 32M | WiFi Router | 580 | 32 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbt-we826-32M-universal-sysupgrade.bin)
ZBT | WE1026-5G  | WiFi Router | 580 | 16,microSD | 64 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/we1026-5g-16m-universal-sysupgrade.bin)
ZBT | WE1326  | WiFi Router | 880 | 16 | 512 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbt-we1326-universal-sysupgrade.bin)
ZBT | WE3526  | WiFi AP | 880 | 16 | 512 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbtlink_zbt-we3526-universal-sysupgrade.bin)
ZBT | WG2626 v03 | WiFi Router | 880 | 16 | 512 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbt-wg2626-universal-sysupgrade.bin)
ZBT | WG3526 16M | WiFi Router | 880 | 16 | 512 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbt-wg3526-16M-universal-sysupgrade.bin)
ZBT | WG3526 32M | WiFi Router | 880 | 32 | 512 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zbt-wg3526-32M-universal-sysupgrade.bin)
ZyXEL | Keenetic Viva rev. B | WiFi Router | 580 | 16 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/kng_rc-universal-sysupgrade.bin)
ZyXEL | Keenetic Extra II  | WiFi Router | 580 | 32 | 128 | [universal](https://github.com/xchwarze/wifi-pineapple-cloner-builds/blob/main/releases/zyxel_keenetic-extra-ii-universal-sysupgrade.bin)
<br>

If your manufacturer or model is not built you have to follow the steps of the Universal Wifi pineapple hardware cloner [documentation](https://github.com/xchwarze/wifi-pineapple-cloner).


## Recomended setup

1. [GL-AR150](https://www.gl-inet.com/products/gl-ar150/) or [GL-AR750S](https://www.gl-inet.com/products/gl-ar750s)
1. USB 2.0 [2 ports hub](https://www.ebay.com/itm/144520475350)
1. Generic [RT5370 WIFI adapter](https://www.ebay.com/itm/284904442887) or [MT7612U WIFI adapter](https://www.ebay.com/itm/175219205235) **you're really going to need this on hardware that doesn't have two wifi adapters**
1. Please support Hak5 work and buy the original hardware!


## If you want to collaborate with hardware 

Those who want to help buy testing hardware or just give me a tip can do so by sending donations to my binance account:

![binance-qr](https://raw.githubusercontent.com/xchwarze/wifi-pineapple-cloner/master/assets/binance-qr.png)
