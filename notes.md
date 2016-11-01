# Notes

- Install ubuntu server w/ ethernet connection

## Wifi

- nmcli not installed by default: `sudo apt install -y network-manager`
- `Error: NetworkManager is not running`: `sudo /etc/init.d/network-manager start`
- `sudo apt install -y wireless-tools`
- `nmtui`: network-manager terminal interface

http://askubuntu.com/questions/461825/connect-to-wifi-from-command-line

Wifi stuck: `sudo service network-manager restart`

## Systemd

### A start job is running for raise network interfaces

`sudo vi /etc/systemd/system/network-online.targets.wants/networking.service`

Then set `TimeoutStartSec=30sec`


## Lightdm

`sudo vim /etc/lightdm/lightdm.conf`

Then write:

```
[SeatDefaults]
greeter-session=lightdm-kde-greeter
```

## Feh (wallpaper manager)

https://www.reddit.com/r/archlinux/comments/3vzd1c/cannot_set_background_in_i3_using_feh/

## Compton

https://wiki.archlinux.org/index.php/Compton
https://bbs.archlinux.org/viewtopic.php?id=117543

## Terminals

### rxvt

https://wiki.archlinux.org/index.php/rxvt-unicode

Transparency https://bbs.archlinux.org/viewtopic.php?id=117543

## GCC

sudo apt install -y gcc-5 g++-5
