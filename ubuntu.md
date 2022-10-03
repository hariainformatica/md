# Ubuntu
Commands used with Ubuntu

## Ubuntu Server
### VirtualBox
#### Install Guest Additions CD Image
```
sudo apt install -y build-essential linux-headers-$(uname -r)
```

copy from

```
https://www.itzgeek.com/post/how-to-install-virtualbox-guest-additions-on-ubuntu-20-04/
```

Mount the ISO to /media directory
```
sudo mount /dev/cdrom /media
```

Execute VirtualBox guest addition installer
```
cd /media
sudo ./VBoxLinuxAddtions.run
```

Reboot your system
```
sudo reboot
```