# Drives
## fix read only usb
### mount as rw
```
mount -w /dev/<device> mnt/
```
### turn off write protection
```
hdparm -r0 /dev/<device>
```

## zero out harddisk (dangerous command)
```
sudo dd if=/dev/zero of=/dev/<device> status=progress
```
Tags: drives, disk, usb, harddisk, ssd, hdd
