grep "CLUE" crimescene
CLUE: Footage from an ATM security camera is blurry but shows that the perpetrator is a tall male, at least 6'.
CLUE: Found a wallet believed to belong to the killer: no ID, just loose change, and membership cards for AAA, Delta SkyMiles, the local library, and the Museum of Bash History. The cards are totally untraceable and have no name, for some reason.
CLUE: Questioned the barista at the local coffee shop. He said a woman left right before they heard the shots. The name on her latte was Annabel, she had blond spiky hair and a New Zealand accent.

grep -R Annabel .
./crimescene:CLUE: Questioned the barista at the local coffee shop. He said a woman left right before they heard the shots. The name on her latte was Annabel, she had blond spiky hair and a New Zealand accent.
./memberships/AAA:Annabel Church
./memberships/AAdvantage:Annabel Fuglsang
./memberships/AAdvantage:Annabel Church
./memberships/Fitness_Galaxy:Oluwasegun Annabel
./memberships/Fitness_Galaxy:Annabel Church
./memberships/Museum_of_Bash_History:Annabel Church
./memberships/Museum_of_Bash_History:Oluwasegun Annabel
./memberships/REI:Annabel Church
./memberships/Rotary_Club:Annabel Sun
./memberships/Rotary_Club:Annabel Fuglsang
./memberships/Rotary_Club:Annabel Church
./people:Annabel Sun	F	26	Hart Place, line 40
./people:Oluwasegun Annabel	M	37	Mattapan Street, line 173
./people:Annabel Church	F	38	Buckingham Place, line 179
./people:Annabel Fuglsang	M	40	Haley Street, line 176
./vehicles:Owner: Oluwasegun Annabel
./vehicles:Owner: Annabel Church
./vehicles:Owner: Annabel Sun
./vehicles:Owner: Annabel Fuglsang

➜  mystery git:(master) ✗ grep "Annabel" -C3 vehicles
License Plate 9R7TTGF
Make: Volkswagen
Color: Yellow
Owner: Oluwasegun Annabel
Height: 5'1"
Weight: 240 lbs



--
--
License Plate L2E48EF
Make: BMW
Color: Orange
Owner: Annabel Church
Height: 5'5"
Weight: 201 lbs

--
--
License Plate 0O27BTD
Make: Fiat
Color: Yellow
Owner: Annabel Sun
Height: 5'0"
Weight: 232 lbs

--
--
License Plate 20VVU2P
Make: Mazda
Color: Pink
Owner: Annabel Fuglsang
Height: 5'11"
Weight: 241 lbs

➜  mystery git:(master) ✗ grep -R INTERVIEW streets 
streets/Alpine_Street:SEE INTERVIEW #862173
streets/Andover_Road:SEE INTERVIEW #904020
streets/Buckingham_Place:SEE INTERVIEW #699607
streets/Cardinal_Medeiros_Avenue:SEE INTERVIEW #141030
streets/Cardington_Street:SEE INTERVIEW #55435298
streets/Claybourne_Street:SEE INTERVIEW #1767435
streets/Culbert_Street:SEE INTERVIEW #2939888
streets/Dalton_Street:SEE INTERVIEW #706620
streets/Dunstable_Road:SEE INTERVIEW #9620713
streets/Fayston_Street:SEE INTERVIEW #3804339
streets/Haley_Street:SEE INTERVIEW #871877
streets/Harbor_Point_Boulevard:SEE INTERVIEW #628618
streets/Hart_Place:SEE INTERVIEW #47246024
streets/Lovis_Street:SEE INTERVIEW #56892213
streets/Manton_Terrace:SEE INTERVIEW #30259493
streets/Mattapan_Street:SEE INTERVIEW #9437737
streets/Plainfield_Street:SEE INTERVIEW #29741223
streets/Richard_Avenue:SEE INTERVIEW #9346061
streets/Rosaria_Street:SEE INTERVIEW #476744
streets/Rozella_Street:SEE INTERVIEW #174898
streets/Senders_Court:SEE INTERVIEW #290346
streets/Terrace_Place:SEE INTERVIEW #82705993
streets/Topeka_Street:SEE INTERVIEW #737609
streets/Trapelo_Street:SEE INTERVIEW #5455315
streets/Wentworth_Street:SEE INTERVIEW #79667499

➜  mystery git:(master) ✗ cat interviews/interview-699607
Interviewed Ms. Church at 2:04 pm.  Witness stated that she did not see anyone she could identify as the shooter, that she ran away as soon as the shots were fired.

However, she reports seeing the car that fled the scene.  Describes it as a blue Honda, with a license plate that starts with "L337" and ends with "9"%                                                                                 ➜  mystery git:(master) ✗ cat interviews/interview-871877
Mr. Fuglsang is male and has brown hair.  Not the witness from the cafe.%                                           ➜  mystery git:(master) ✗ cat interviews/interview-4726024
cat: interviews/interview-4726024: No such file or directory
➜  mystery git:(master) ✗ cat interviews/interview-47246024 
Ms. Sun has brown hair and is not from New Zealand.  Not the witness from the cafe.%                                ➜  mystery git:(master) ✗ cat interviews/interview-9437737 
Doesn't appear to be the witness from the cafe, who is female.%   

➜  mystery git:(master) ✗ grep -A 5 "L337" vehicles | grep -A 1 -B 4 "6'" | grep -A 4 -B 1 "Honda" | grep -A 3 -B 2 "Blue"
License Plate L337QE9
Make: Honda
Color: Blue
Owner: Erika Owens
Height: 6'5"
Weight: 220 lbs
--
--
License Plate L337DV9
Make: Honda
Color: Blue
Owner: Joe Germuska
Height: 6'2"
Weight: 164 lbs
--
--
License Plate L3375A9
Make: Honda
Color: Blue
Owner: Jeremy Bowers
Height: 6'1"
Weight: 204 lbs
--
--
License Plate L337WR9
Make: Honda
Color: Blue
Owner: Jacqui Maher
Height: 6'2"
Weight: 130 lbs

➜  mystery git:(master) ✗ grep -R "Joe Germuska" memberships
memberships/AAA:Joe Germuska
memberships/Terminal_City_Library:Joe Germuska
➜  mystery git:(master) ✗ grep -R "Jeremy Bowers" memberships
memberships/AAA:Jeremy Bowers
memberships/Delta_SkyMiles:Jeremy Bowers
memberships/Museum_of_Bash_History:Jeremy Bowers
memberships/Terminal_City_Library:Jeremy Bowers
➜  mystery git:(master) ✗ grep -R "Jacqui Maher" memberships
memberships/AAA:Jacqui Maher
memberships/Delta_SkyMiles:Jacqui Maher
memberships/Museum_of_Bash_History:Jacqui Maher
memberships/Terminal_City_Library:Jacqui Maher

➜  mystery git:(master) ✗ grep "Jeremy Bowers" people 
Jeremy Bowers	M	34	Dunstable Road, line 284
➜  mystery git:(master) ✗ grep "Jacqui Maher" people 
Jacqui Maher	F	40	Andover Road, line 224
➜  mystery git:(master) ✗ grep "Erika Owens" people 
Erika Owens	F	56	Trapelo Street, line 98

Jeremy Bowers