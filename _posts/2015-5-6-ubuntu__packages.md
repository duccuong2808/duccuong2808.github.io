---
layout: post
author: NDC
title: Ubuntu package
excerpt_separator: <!--more-->
tags:
    - ubuntu
    - package
---

Danh sách các package dành cho Ubuntu

- [uGet, the Best Download Manager for Linux](#uget-the-best-download-manager-for-linux)
- [Wifi for Ubuntu](#wifi-for-ubuntu)
- [Apt-fast](#apt-fast)
- [Dukto](#dukto)
- [Shuttter](#shutter)
- [Nemo](#nemo)
- [Xkbmod Indicator](#xkbmod-indicator)
- [Pushbullet](#pushbullet)
- [Other Software](#other-software)


##### uGet, the Best Download Manager for Linux.
[http://ugetdm.com/](http://ugetdm.com/)

##### Wifi for Ubuntu

Install ap-hotspot

```bash
    sudo add-apt-repository ppa:nilarimogard/webupd8
    sudo apt-get update
    sudo apt-get install ap-hotspot
```
command:

```bash
    sudo ap-hotspot start
    sudo ap-hotspot configure
    sudo ap-hotspot stop
    sudo ap-hotspot restart
```

- - -

##### apt-fast

*Use apt-fast instead of apt-get for a speedy update:*
>`apt-fast` is a shellscript wrapper for “apt-get” that improves updated and package download speed by downloading packages from multiple connection simultaneously.
If you frequently use terminal and apt-get to install and update the packages, you may want to give apt-fast a try.

Install `apt-fast` via official PPA using the following commands:

```bash
    sudo add-apt-repository ppa:apt-fast/stable
    sudo apt-get update
    sudo apt-get install apt-fast
```
- - -

##### DUKTO

> Dukto R6 is an open source, multi-platform LAN file transfer tool, useful to transfer files form one computer to another without having to worry about configurations, operating systems, clients, servers and so on.

Link : [http://www.msec.it/blog/?page_id=11](http://www.msec.it/blog/?page_id=11)

Dukto R6 features:

	* supports sending and receiving files or folders as well as text snippets on your LAN;
	* multi-platform;
	* multi-transfer support;
	* zero configuration;
	* clients auto-discovery;
	* transfers log;
	* shows your IP addresses on the IP connection page;
	* full Unicode support;
	* Windows 7 taskbar integration with progress and transfer indicator;
	* Metro style UI with configurable colors.

Install for Ubuntu:

```bash
    sudo sh -c "echo 'deb http://download.opensuse.org/repositories/home:/colomboem/xUbuntu_13.10/ /' >> /etc/apt/sources.list.d/dukto.list"
    sudo apt-get update
	sudo apt-get install dukto
```

- - -
##### Shutter
> Shutter is one of the most versatile screenshot utilities available for Linux, with an open-source feature set letting you capture shots of your desktop, windowed apps and menus, plus edit, crop and add annotations, text and other visual effects to them.

```bash
	sudo add-apt-repository ppa:shutter/ppa
	sudo apt-get update && sudo apt-get install shutter
```
Source: http://www.omgubuntu.co.uk/2014/08/shutter-0-9-2-released-removes-ubuntu-one

- - -

#####Nemo
http://www.webupd8.org/2014/08/nemo-emblems-folder-color-image.html

- - -

#####Xkbmod Indicator
Keyboard Modifiers State indicator For Ubuntu

[Webupd8](http://www.webupd8.org/2014/09/keyboard-modifiers-state-indicator-for.html)

#####Pushbullet

http://www.webupd8.org/2014/09/pushbullet-indicator-gets-partial.html

#####Rcconf

```bash
sudo  apt-get install rcconf
```

Rcconf is another runlevel configuration tool tool having the same functionalities as BUM, but it can be run only via the terminal, no GUI

#####Other Software
okular

+ okular : pdf reader

