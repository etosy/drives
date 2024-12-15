# Drives
## fix read only usb
### mount as rw
```
mount -w /dev/<device> /mnt
```
### turn off write protection (worked 2 times)
```
hdparm -r0 /dev/<device>
```

## zero out harddisk (dangerous command, if this not worked, it may be encrypted)
```
sudo dd if=/dev/zero of=/dev/<device> status=progress
```
Tags: drives, disk, usb, harddisk, ssd, hdd
