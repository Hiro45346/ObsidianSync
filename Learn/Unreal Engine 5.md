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
Hot Key on Viewport scene
	Select object on outliner + F-Key -> Focus on the actor
	R-Key -> Scale Actor
	E-Key -> Rotate Actor
	W-Key -> move Actor
		Or space bar -> Switch between all of these (R, E and W)
	Hold Alt + move actor -> Duplicate actor
	End Key -> Snap actor to surface
	