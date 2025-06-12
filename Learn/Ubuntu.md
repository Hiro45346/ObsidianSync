### Reset password 
```linux title:1.CheckUsername
ls home/ 
```

``` title:2.MountFileWriteable
mount -o remount,rw /
```

``` title:2.ResetPasswd
passwd yourusername
```

``` title:CheckGPUandMotherboard
sudo dmidecode -t system
lspci | grep -i vga
sudo lshw -c video
```