mystery/
ls
grep "CLUE" crimescene
<!-- CLUE: Footage from an ATM security camera is blurry but shows that the perpetrator is a tall male, at least 6'.
CLUE: Found a wallet believed to belong to the killer: no ID, just loose change, and membership cards for AAA, Delta SkyMiles, the local library, and the Museum of Bash History. The cards are totally untraceable and have no name, for some reason.
CLUE: Questioned the barista at the local coffee shop. He said a woman left right before they heard the shots. The name on her latte was Annabel, she had blond spiky hair and a New Zealand accent. -->
people
cat people
grep "Annabel" people
<!-- Annabel Sun	F	26	Hart Place, line 40
Oluwasegun Annabel	M	37	Mattapan Street, line 173
Annabel Church	F	38	Buckingham Place, line 179 
Annabel Fuglsang	M	40	Haley Street, line 176 -->
head people
<!-- To go to the street someone lives on, use the file
for that street name in the 'streets' subdirectory.
To knock on their door and investigate, read the line number
they live on from the file.  If a line looks like gibberish, you're at the wrong house.
***************

NAME	GENDER	AGE	ADDRESS
Alicia Fuentes	F	48	Walton Street, line 433
Jo-Ting Losev	F	46	Hemenway Street, line 390 -->
head -n 173 streets/Mattapan_Street | tail -n 1
<!-- SEE INTERVIEW #9437737 -->

cat interviews/interview-9437737 
<!-- Doesn't appear to be the witness from the cafe, who is female.%  -->

head -n 40 streets/Hart_Place | tail -n 1
<!-- SEE INTERVIEW #47246024 -->

cat interviews/interview-47246024
<!-- Ms. Sun has brown hair and is not from New Zealand.  Not the witness from the cafe.%  -->

 head vehicles 
<!-- ***************
Vehicle and owner information from the Terminal City Department of Motor Vehicles
***************

License Plate T3YUHF6
Make: Toyota
Color: Yellow
Owner: Jianbo Megannem
Height: 5'6"
Weight: 246 lb -->s

grep -A 5 "L337" mystery/vehicles

<!-- License Plate L337ZR9
Make: Honda
Color: Red
Owner: Katie Park
Height: 6'2"
Weight: 189 lbs -->
<!-- One of these guys could be the criminal -->
--
<!-- License Plate L337GX9
Make: Mazda
Color: Orange
Owner: John Keefe
Height: 6'4"
Weight: 185 lbs
-- -->
<!-- License Plate L337QE9
Make: Honda
Color: Blue
Owner: Erika Owens
Height: 6'5"
Weight: 220 lbs -->
--
License Plate L337GB9
Make: Toyota
Color: Blue
Owner: Matt Waite
Height: 6'1"
Weight: 190 lbs
--
License Plate L337OI9
Make: Jaguar
Color: Blue
Owner: Brian Boyer
Height: 6'6"
Weight: 201 lbs
--
<!-- License Plate L337X19
Make: Fiat
Color: Blue
Owner: Al Shaw
Height: 6'5"
Weight: 240 lb -->s
--
<!-- License Plate L337539
Make: Honda
Color: Blue
Owner: Aron Pilhofer
Height: 5'3"
Weight: 198 lbs -->
--
<!-- License Plate L3373U9
Make: Ford
Color: Blue
Owner: Miranda Mulligan
Height: 6'6"
Weight: 156 lbs -->
--
<!-- License Plate L337369
Make: Honda
Color: Blue
Owner: Heather Billings
Height: 5'2"
Weight: 244 lbs -->
--
<!-- License Plate L337DV9
Make: Honda
Color: Blue
Owner: Joe Germuska
Height: 6'2"
Weight: 164 lbs -->
--
License Plate L3375A9
Make: Honda
Color: Blue
Owner: Jeremy Bowers
Height: 6'1"
Weight: 204 lbs
--
<!-- License Plate L337WR9
Make: Honda
Color: Blue
Owner: Jacqui Maher
Height: 6'2"
Weight: 130 lbs -->

memberships
cat AAA Delta_SkyMiles Museum_of_Bash_History Terminal_City_Library | grep "John Keefe"
<!-- John Keefe
John Keefe -->

cat AAA Delta_SkyMiles Museum_of_Bash_History Terminal_City_Library | grep "Matt Waite"
<!-- Matt Waite
Matt Waite
Matt Waite
Matt Waite -->

at AAA Delta_SkyMiles Museum_of_Bash_History Terminal_City_Library | grep "Brian Boyer"
<!-- Brian Boyer
Brian Boyer
Brian Boyer
Brian Boye -->r

cat AAA Delta_SkyMiles Museum_of_Bash_History Terminal_City_Library | grep "Al Shaw" 
<!-- Al Shaw
Al Shaw -->

cat AAA Delta_SkyMiles Museum_of_Bash_History Terminal_City_Library | grep "Joe Germuska"
<!-- Joe Germuska
Joe Germuska -->

cat AAA Delta_SkyMiles Museum_of_Bash_History Terminal_City_Library | grep "Jeremy Bowers"
<!-- Jeremy Bowers
Jeremy Bowers
Jeremy Bowers
Jeremy Bowers -->


<!-- 3 Guys that could be the criminal, but Jeremy Bowers has a Honda that is Blue, so it's Jeremy Bowers. 

License Plate L337GB9
Make: Toyota
Color: Blue
Owner: Matt Waite
Height: 6'1"
Weight: 190 lbs
--
License Plate L337OI9
Make: Jaguar
Color: Blue
Owner: Brian Boyer
Height: 6'6"
Weight: 201 lbs

License Plate L3375A9
Make: Honda
Color: Blue
Owner: Jeremy Bowers
Height: 6'1"
Weight: 204 lbs -->






