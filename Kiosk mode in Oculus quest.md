check all devices
adb devices

disbled home
adb -s <device ID> shell pm disable-user --user 0 com.oculus.vrshell

enabled home
adb -s <device ID> shell pm enable com.oculus.vrshell