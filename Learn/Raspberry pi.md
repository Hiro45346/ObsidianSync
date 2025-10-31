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

Calibrate LED scale
```Python title:Calibrate
		self.screen.set_at((0,0),(255,0,0))
        pygame.draw.rect(self.screen, (255,0,0), pygame.Rect(0,0,512,128),1)
```

Set Rasp-pi resolution
``` title:wlr-randr.cmd
	#Check monitor resolution
	wlr-randr
```


## Auto start script
1.  Make auto run script
``` title:CreateAutorunFile
	nano /home/<folder name>/<file name>.sh
	
    #Add this script to file
    
	# Wait for the desktop/compositor to be fully up
	sleep 2

	# Make SDL/Pygame use X11 (exact pixel mapping) and start at (0,0)
	export DISPLAY=:0
	export SDL_VIDEODRIVER=x11
	export SDL_VIDEO_CENTERED=0
	export SDL_VIDEO_WINDOW_POS=0,0

	# Run your app (edit the path to your .py file if different)
	exec /usr/bin/python3 /home/<folder name>/<file name>.py	
	
```

2. Config desktop auto run
``` title:ConfigAutostart
	
	mkdir -p ~/.config/autostart
	nano ~/.config/autostart/scene-viewer.desktop
	
	#Add this script to file
	[Desktop Entry]
	Type=Application
	Name=Scene Viewer
	Comment=Auto-start Pygame scene viewer
	Exec=/bin/bash -lc '/home/<folder name>/<file name>.sh'
	X-GNOME-Autostart-enabled=true
 

```

3. reboot Rasp-pi 
```
	sudo reboot
```