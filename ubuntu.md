# Ubuntu
Commands used with Ubuntu

## Ubuntu Server

### Keyboard
Change keyboard to spanish layout
```
sudo loadkeys es
```
This command change the layout for the actua session

To change the layout for default edit the file
```
/etc/default/keyboard
```

### Users
Add user
```
$ sudo adduser username
```

If you want the newly created user to have administrative rights
```
$ sudo usermod -aG sudo username
```

### Hostname
/etc/hostname
/etc/hosts


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