## Download and install software to micro SD card
1. Click this link https://www.raspberrypi.com/software/ 
2. Connect micro SD card to PC.
3. Download and in stall file to micro SD card

## Open raspberry pi and setting 
1. Open terminal and type this
```python title:python(gpiozero)
sudo apt update
sudo apt install python3-gpiozero
```

## Test button
```
nano test_button.py
```

Key shortcut
	Press **CTRL + O** -> Enter (to save)
	Press **CTRL+X** (to exit nano).
Used open framework
1. download open framework for arm64
2. Extract folder to /home
3. install it
```
cd ~/of_v0.12.0_linuxaarch64_release/scripts/linux
sudo ./install_dependencies.sh
sudo ./install_codecs.sh
```
1. 
``` title:RunOnBoot
python3 <Path file> --> python3 /home/esic/test_button.py

sudo crontab -e --> use recomented method

@reboot <Path file> &
```