# friWrt-builder | OpenWrt and ImmortalWrt

### What's this?
This is a openwrt toolchain called Image Builder to build a pre-compiled image to ready one firmware. You can customize your own packages adn custom files that suitable for you. 

Using [MyWrtBuilder](https://github.com/Revincx/MyWrtBuilder) from Revincx as source base scripts, by adopting and improve it by adding ability to chose Source and Branch version, feature to easy change rootfs partition size, flexible target device, improve logic code and much more.

By default, im using Raspberry Pi 4B device with all my preference packages and custom files configuration was placed here.

### Features of this project
* Using ImageBuilder to build firmware saves time and effort. It only takes less than half an hour to build once.
* It has built-in Luci software packages that I use daily, and can be used almost out of the box.
* The latest version of Clash kernel is built-in using auto download latest core script, no need to download it yourself.
* Built-in Docker and AdGuard Home components, no complex configuration required.
* Simply modify make-build.sh to build your own firmware for easy customization.

### How To
Select for using Official OpenWrt or ImmortalWrt as a source base and branch version with just one click!

You can also edit the package you want by simply edit "make-build.sh" file!

Want to use custom .ipk packages or custom files?
Put the url link on "external-package-urls.txt" or upload it to "packages" folder, then write down the ipk package name on "make-buil.sh".
Custom files or configuration on "files" folder.
Please read instruction given.

### Firmware details

Login info
* 192.168.1.1 | user: root | password: friwrt
* SSID: friWrt_5g | password: friwrt

- AdGuard Home installed and enable (disable using "adguardhome disable" command on terminal, and "adguardhome enable" to enable again),
- Openclash with latest core and latest MetaCubeX Mihomo core,
- DOCKER installed, ready to run container,
- Aria2 download server,
- SAMBA4 server for sharing storage,
- TinyFm file manager,
- Internet Detector and Watchcat,
- vnstat2 and Nlbwmon for Bandwith Monitoring,
- Argon Theme with some cool custom login image,
- Modemmanager protocol for connecting 4g/5g modems (im using Dell DW5821e Snapdragon X20 LTE)
- OLED Display support (only Raspberrry Pi 4B tested),
- and other that i forgot to mention ~

you can find my done build on Release.

### Acknowledgments

[MyWrtBuilder](https://github.com/Revincx/MyWrtBuilder)

[OpenWrt](https://github.com/openwrt/openwrt/)

[ImmortalWrt](https://github.com/immortalwrt/immortalwrt)

[Image Builder Docs](https://openwrt.org/docs/guide-user/additional-software/imagebuilder)

[GitHub Actions](https://github.com/features/actions)
