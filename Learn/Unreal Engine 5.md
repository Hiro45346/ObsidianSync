For movement use 
```C++ title:In.h
	void MoveForward(float value);
	void MoveRight(float value);
```

``` C++ title:In.cppFile
	PlayerInputConponent->BindAxis("MoveForward", this,  &ASCharacter::MoveForward);
	PlayerInputComponent->BindAxis("Right", this, &ASCharacter::Right);	 
```

For Turn or Rotation use
``` C++ title:In.cppFile
	PlayerInputConponent->BindAxis("lookUp", this,  &APawn::AddControllerPitchInput); //For Y axis 
	PlayerInputConponent->BindAxis("Turn", this,  &APawn::AddControllerYawInput); //For X axis
```

Hot Key on UE5
	Ctrl + N -> Create new level
	Ctrl + Shift +S -> Save everything (Recommendation)
	Alt + P -> Enter play mode
	Alt + S -> Enter simulation mode
	Alt + C -> Show all collision in scene
	Select object on outliner or content drawer + Ctrl + E-Key -> Open selected item blueprint  
Hot Key on Viewport scene
	Select object on outliner + F-Key -> Focus on the actor
	R-Key -> Scale Actor
	E-Key -> Rotate Actor
	W-Key -> move Actor
		Or space bar -> Switch between all of these (R, E and W)
	Hold Alt + move actor -> Duplicate actor
	End Key -> Snap actor to surface
	Ctrl + (1, 2, ...) -> Create camera bookmark
	1, 2, ... Key -> Show camera bookmark
	Shift + F11-Key -> Editor full screen mode
	F11-Key -> immersive mode
	G-Key -> Toggle game mode
	Ctrl + Shift + T-Key -> Toggle tools visibility
	Ctrl + Shift + H-Key -> Toggle frame rate
	Select object on outliner + Ctrl + G-Key -> Group actors
	Select object on outliner + Shift + G-Key -> Ungroup actors
	Shift + (1, 2, ...) -> Change editor mode
Hot Key on Content
	Ctrl + Space bar -> Open content drawer
	Select object on outliner + Ctrl + B-Key -> find object in content
	Ctrl + Shift + N-Key -> Create New folder
	Ctrl + D-Key -> Duplicate Item 
	F2-Key -> Rename
	