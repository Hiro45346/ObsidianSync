For movement use 
	 In .h
	 ```void MoveForward(float value);
	 void MoveRight(float value);```
	 In .CPP file 
	 ```PlayerInputConponent->BindAxis("MoveForward", this,  &ASCharacter::MoveForward);
	 PlayerInputComponent->BindAxis("Right", this, &ASCharacter::Right);
	 ```
For Turn or Rotation use
	 In .CPP file 
	 ```PlayerInputConponent->BindAxis("lookUp", this,  &APawn::AddControllerPitchInput); //For Y axis 
	 PlayerInputConponent->BindAxis("Turn", this,  &APawn::AddControllerYawInput); //For X axis
	 ```




