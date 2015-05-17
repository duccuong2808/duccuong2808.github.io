---
layout: post
author: NDC
excerpt_separator: <!--more-->
---

This is packages and tip for ubuntu

- [List all Installed Packages](#list-all-installed-packages)
- [Data size of folder](#data-size-of-folder)
- [Change SSH config](#change-ssh-config)
- [Remove repository via terminal](#remove-repository-via-terminal)
- [Refresh hosts file without rebooting](#linux--how-to-refresh-hosts-file-without-rebooting)
- [Change repo source.list use terminal](#change-repo-sourcelist-use-terminal)



##### List all Installed Packages

Here less = fix in a page to scroll

```bash
	dpkg -l | less
```

To check Wether the package installed are not

syntax :

```bash
  dpkg -l {package_name}
  dpkg -l vlc
```

To check the Package Wether installed are not and if there is package installed it need to get launched

```bash
  dpkg -l | vlc
```

To see Wether the package installed or not.

And this will show the Location were else it have installed Here -S (Captial S) to Search the package installed or not

```bash
  sudo dpkg -S {package_name}
  sudo dpkg -S skype
```

And we can Even Use a Grep Command as follow by listing

```bash
  dpkg -l | grep linux-image
```

- - -

#####  Data size of folder

```bash
  sudo du -h s *
```
or

```bash
du -h --max-depth=1
```

##### Change SSH config
Edit file

```bash
  sudo vim /etc/ssh/sshd_config
```

```bash
  sudo /etc/init.d/ssh start
  sudo /etc/init.d/ssh stop
  sudo /etc/init.d/ssh restart
  #  OR
  sudo service ssh start
  sudo service ssh stop
  sudo service ssh restart


  sudo service ssh status
```

- - -

##### Remove repository via terminal?!

   ```bash
    ls /etc/apt/sources.list.d/*.list
    # Remove
    rm /etc/apt/sources.list.d/name_respository.list
   ```
- - -
##### Linux – How to refresh hosts file without rebooting

After editing the /etc/hosts file you don’t need to reboot the machine.
you can do it as follows for debian:

```bash
	sudo /etc/init.d/networking restart
```
and as follows for redhat flavors:

```bash
	sudo service networking restart
```
After,for firefox, restart firefox. And for chrome,go to `chrome://net-internals/#dns` and click “Clear host cache”.

- - -

##### Change repo source.list use terminal

old repo: `http://archive.ubuntu.com/ubuntu`
new repo: `http://ubuntu.01link.hk/`

change

```bash
sudo sed -i 's/http:\/\/archive.ubuntu.com\/ubuntu/http:\/\/ubuntu.01link.hk\//g' /etc/apt/sources.list
```

restore

```bash
sudo sed -i 's/http:\/\/ubuntu.01link.hk\//http:\/\/archive.ubuntu.com\/ubuntu/g' /etc/apt/sources.list
```
-----


##### Other tip

```bash
sudo rm -r /var/lib/apt/lists/*
sudo rm /var/lib/dpkg/lock
sudo rm /var/cache/apt/archives/lock

sudo dpkg --configure -a

sudo apt-get update

```