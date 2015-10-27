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

		preliminary conclusion: witness is Annabel Church.Annabel Church	F	38	Buckingham Place, line 179	


from the Lead: Find a be Honda plates L337 ending in 9
	grep "L337" vehicles
License Plate L337ZR9
License Plate L337P89
License Plate L337GX9
License Plate L337QE9
License Plate L337GB9
License Plate L337OI9
License Plate L337X19
License Plate L337539
License Plate L3373U9
License Plate L337369
License Plate L337DV9
License Plate L3375A9
License Plate L337WR9
	
	to get more info for 5 lines following each line matching license plate number
		grep -A 5 "L337" vehicles
	suspects fitting description of tall male (>6’0), with blue Honda:

		License Plate L337DV9
		Make: Honda
		Color: Blue
		Owner: Joe Germuska
		Height: 6'2"
		Weight: 164 lbs
		
		License Plate L3375A9
		Make: Honda
		Color: Blue
		Owner: Jeremy Bowers
		Height: 6'1"
		Weight: 204 lbs.



	cross reference the memberships with the two names of suspects. Inside Memberships folder
	cat AAA Delta_SkyMiles Terminal_city_library Museum_of_Bash_History | grep "Joe Germuska"
		2 results positive

	cat AAA Delta_SkyMiles Terminal_city_library Museum_of_Bash_History | grep "Jeremy Bowers"
		ALL 4 RESULTS ARE POSITIVE.





Suspect Identified as Jeremy Bowers  


		