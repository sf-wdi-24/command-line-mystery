cd mystery
ls
grep -R “CLUE” ./


RESULTS:
.//crimescene:CLUE: Footage from an ATM security camera is blurry but shows that the perpetrator is a tall male, at least 6'.
.//crimescene:CLUE: Found a wallet believed to belong to the killer: no ID, just loose change, and membership cards for AAA, Delta SkyMiles, the local library, and the Museum of Bash History. The cards are totally untraceable and have no name, for some reason.
.//crimescene:CLUE: Questioned the barista at the local coffee shop. He said a woman left right before they heard the shots. The name on her latte was Annabel, she had blond spiky hair and a New Zealand accent.


cat people
grep -R “Annabel” ./


RESULTS:
.//memberships/AAA:Annabel Church
.//memberships/AAdvantage:Annabel Church
.//memberships/Fitness_Galaxy:Annabel Church
.//memberships/Museum_of_Bash_History:Annabel Church
.//memberships/REI:Annabel Church
.//memberships/Rotary_Club:Annabel Church
.//people:Annabel Church	F	38	Buckingham Place, line 179
.//vehicles:Owner: Annabel Church
 

cd streets
cat Buckingham Place  

RESULTS:
SEE INTERVIEW #699607



cd ../
cd interviews
cat interview-699607

RESULTS:
Interviewed Ms. Church at 2:04 pm.  Witness stated that she did not see anyone she could identify as the shooter, that she ran away as soon as the shots were fired.

However, she reports seeing the car that fled the scene.  Describes it as a blue Honda, with a license plate that starts with "L337" and ends with "9"



cd ../
cd vehicles
egrep -A5 -B1 "L337" "vehicles-Make: Honda" "vehicles-Color: Blue" vehicles

RESULTS:
vehicles-
vehicles:License Plate L337DV9
vehicles-Make: Honda
vehicles-Color: Blue
vehicles-Owner: Joe Germuska
vehicles-Height: 6'2"
vehicles-Weight: 164 lbs

vehicles-
vehicles:License Plate L3375A9
vehicles-Make: Honda
vehicles-Color: Blue
vehicles-Owner: Jeremy Bowers
vehicles-Height: 6'1"
vehicles-Weight: 204 lbs



cd ../
cd mystery
cd memberships
egrep -R -A5 -B1 “Jeremy Bowers” ./

RESULTS
(has all memberships)
.//memberships/AAA
.//memberships/Delta_SkyMiles
.//memberships/Museum_of_Bash_History
.//memberships/Terminal_City_Library
--
.//people:Jeremy Bowers	M	34	Dunstable Road, line 284



cd streets
ls
cat Dunstable_Road


RESULTS:
SEE INTERVIEW #9620713



cd ../
cd interviews
ls
cat interview-9620713


RESULTS:
Home appears to be empty, no answer at the door.

After questioning neighbors, appears that the occupant may have left for a trip recently.

Considered a suspect until proven otherwise, but would have to eliminate other suspects to confirm.



Jeremy Bowers is my final answer...








