![OpenIPC logo][logo]

## OpenIPC Builder
**_Experimental system for building OpenIPC firmware for known devices_**
- **_[Current release of firmware builds](https://github.com/OpenIPC/builder/releases/tag/latest)_**


### Specialized features

- Tweaker for automatically configuring devices according to profile (gpio, wifi, etc).
- Specialized _[storage location](https://github.com/OpenIPC/builder/releases/tag/latest)_ for customized firmware for well-known devices.
- QR code recognition to automatically _[connect to WiFi](https://openipc.org/tools/qr-code-generator)_ on your home network.


### List of known devices

```
Imou IPC-C22EP-S2             SSC325DE       SC2239     RTL8188FU     NAND         in progress
Imou IPC-F22AP                SSC325         SC2239     -             NOR_?        preparation
Rostelecom IPC8232SWC-WE-B    SSC337DE       OS02G10    RTL8188FU     NOR_16M      preparation
Smartwares CIP-37210          HI3518EV200    OV9732     RTL8188FU     NOR_16M      in progress
Switcam HS303                 HI3518EV200    JXF22      RTL8188FU     NOR_16M      in progress
Switcam HS303 v2              HI3518EV200    OV9732     RTL8188EU     NOR_16M      in progress
Switcam HS303 v3              HI3518EV200    OV9732     RTL8188EU     NOR_16M      in progress
TP-Link Tapo C110             SSC333         SC3338     SSW101B       NOR_8M       in progress
Uniview C1L-2WN-G-RU          SSC337DE       OS02G10    RTL8188FU     NOR_16M      preparation

```


### Preparing and using the project

```
sudo apt-get update -y
sudo apt-get install -y automake autotools-dev bc build-essential curl fzf git libtool rsync unzip mc tree python-is-python3
git clone https://github.com/openipc/builder.git
cd builder
./builder.sh
```

### Existing problems

- On some devices NOR flash 8M is small, and the WiFi driver is very large and the QR scanner currently does not fit into the firmware


### Technical support and donations

Please **_[support our project](https://openipc.org/support-open-source)_** with donations or orders for development or maintenance. Thank you!


[logo]: https://openipc.org/assets/openipc-logo-black.svg

