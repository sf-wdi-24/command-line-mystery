grep "CLUE" crimescene
	*CLUE: Footage from an ATM security camera is blurry but shows that the perpetrator is a tall male, at least 6'.
	*CLUE: Found a wallet believed to belong to the killer: no ID, just loose change, and membership cards for AAA, Delta SkyMiles, the local library, and the Museum of Bash History. The cards are totally untraceable and have no name, for some reason.
	*CLUE: Questioned the barista at the local coffee shop. He said a woman left right before they heard the shots. The name on her latte was Annabel, she had blond spiky hair and a New Zealand accent.




Look for Annabel.
  	Head people 
		To go to the street someone lives on, use the file
for that street name in the 'streets' subdirectory.
To knock on their door and investigate, read the line number
they live on from the file.  If a line looks like gibberish, you're at the wrong house.


	Grep “Annabel” people
		2 Females
			Annabel Sun	F	26	Hart Place, line 40
			Annabel Church	F	38	Buckingham Place, line 179


look in streets directory
	head -40 Hart_Place 
		…some gibberish …
		stupendous prolonged smog naps 
			SEE INTERVIEW #47246024
	head -179 Buckingham_Place
		…some gibberish …
		 overheats embittering grimmer beamed 
			SEE INTERVIEW #699607

look in interviews directory
	
	cat interview-47246024
		Ms. Sun has brown hair and is not from New Zealand.  Not the witness from the cafe.
	
	cat interview-699607
		Interviewed Ms. Church at 2:04 pm.  Witness stated that she did not see anyone she could identify as the shooter, that she ran away as soon as the shots were fired.
		However, she reports seeing the car that fled the scene.  Describes it as a blue Honda, with a license plate that starts with "L337" and ends with “9”. 
	