---
layout: post
author: NDC
excerpt_separator: <!--more-->
tag:
    - ubuntu
---


**Use apt-fast instead of apt-get for a speedy update:**

`apt-fast` is a shellscript wrapper for `apt-get` that improves updated and package download speed by downloading packages from multiple connection simultaneously. 

If you frequently use terminal and apt-get to install and update the packages, you may want to give `apt-fast` a try. 

Install apt-fast via official PPA using the following commands:

```bash
sudo add-apt-repository ppa:apt-fast/stable
sudo apt-get update
sudo apt-get install apt-fast
```
```bash
sudo rm -r /var/lib/apt/lists/*
sudo rm /var/lib/dpkg/lock
sudo rm /var/cache/apt/archives/lock

sudo dpkg --configure -a

sudo apt-get update

```

	
**BUBBLE NOTIFY**

Customize Bubble Notifications as you like in Ubuntu 14.04/13.10/12.10/12.04 (PPA)


Add this PPA to get patched NotifyOSD, Enter these commands in terminal:

```bash
sudo add-apt-repository ppa:leolik/leolik
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install libnotify-bin
```

Now install GUI configure NotifyOSD, Enter these commands in terminal to get it:

```bash
sudo add-apt-repository ppa:amandeepgrewal/notifyosdconfig
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install notifyosdconfig
```
	
**Unity Drawers**

Add another feature to your Ubuntu Unity

```bash
sudo add-apt-repository ppa:ian-berke/ppa-drawers
sudo apt-get update
sudo apt-get install drawers
```

**DUKTO**

DUKTO LAN FILE TRANSFER TOOL IS EASY TO USE, MULTI-PLATFORM
Link : [http://www.msec.it/blog/?page_id=11](http://www.msec.it/blog/?page_id=11)

Dukto R6 features:

>	* supports sending and receiving files or folders as well as text snippets on your LAN;

>	* multi-platform;

>	* multi-transfer support;

>	* zero configuration;

>	* clients auto-discovery;

>	* transfers log;

>	* shows your IP addresses on the IP connection page;

>	* full Unicode support;

>	* Windows 7 taskbar integration with progress and transfer indicator;

>	* Metro style UI with configurable colors.

		
