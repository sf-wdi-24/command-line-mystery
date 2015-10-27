* touch solution.md
cat instructions
cd mystery
ls mystery
cd crimescene
ls crimescene
cat crimescene
cat interviews
cat people
cat streets
cat hint4
cat hint5

cd develop
cd command-line-mystery


grep "CLUE" crimescene

CLUE: Footage from an ATM security camera is blurry but shows that the perpetrator is a tall male, at least 6'.
CLUE: Found a wallet believed to belong to the killer: no ID, just loose change, and membership cards for AAA, Delta SkyMiles, the local library, and the Museum of Bash History. The cards are totally untraceable and have no name, for some reason.
CLUE: Questioned the barista at the local coffee shop. He said a woman left right before they heard the shots. The name on her latte was Annabel, she had blond spiky hair and a New Zealand accent.


grep 'Annabel' people
Annabel Sun	F	26	Hart Place, line 40
Oluwasegun Annabel	M	37	Mattapan Street, line 173
Annabel Church	F	38	Buckingham Place, line 179
Annabel Fuglsang	M	40	Haley Street, line 176

head -n 40 streets/Hart_Place
head -n 179 streets/Buckingham_Place

cd interviews
cat interview-699607
cat interview-47246024

grep -A 5 "L337" mystery/vehicles

//POSSIBLE SUSPECTS MATCHING BLUE HONDA & MALE & 6FT TALL

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
Weight: 204 lbs


grep -R "Bowers" memberships                          //MATCHES SUSPECT INFORMATION!!
memberships/AAA:Jeremy Bowers
memberships/Delta_SkyMiles:Jeremy Bowers
memberships/Museum_of_Bash_History:Jeremy Bowers
memberships/Terminal_City_Library:Jeremy Bowers

grep -R "Germuska" memberships
memberships/AAA:Joe Germuska
memberships/Terminal_City_Library:Joe Germuska


SOLUTION: JEREMY BOWERS