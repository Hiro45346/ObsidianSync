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



