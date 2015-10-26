touch solution.md
cat instructions
cd mystery
ls

grep "CLUE" crimescene > clues
cat clues

head people
grep "Annabel" people
	Annabel Sun	F	26	Hart Place, line 40
	Oluwasegun Annabel	M	37	Mattapan Street, line 173
	Annabel Church	F	38	Buckingham Place, line 179
	Annabel Fuglsang	M	40	Haley Street, line 176

cd streets
ls
cd ..

head -n 40 streets/Hart_Place | tail -n 1
	SEE INTERVIEW #47246024

ls interviews

cat interviews/interview-47246024
	Ms. Sun has brown hair and is not from New Zealand.  Not the witness from the cafe.

head -n 173 streets/Mattapan_Street | tail -n 1 
	SEE INTERVIEW #9437737

cat interviews/interview-9437737
	Doesn't appear to be the witness from the cafe, who is female.

head -n 173 streets/Mattapan_Street | tail -n 1 
	SEE INTERVIEW #699607

cat interviews/interview-699607
	Blue Honda - license plate starts with L337, ends with 9

head -n 176 streets/Haley_Street | tail -n 1
	SEE INTERVIEW #871877

cat interviews/interview-871877
	Mr. Fuglsang is male and has brown hair.  Not the witness from the cafe.

head -20 vehicles
grep -A 5 "L337..9" vehicles
	Owner: Joe Germuska
	Owner: Jeremy Bowers
	
ls memberships
cd memberships
cat AAA Delta_SkyMiles Terminal_City_Library Museum_of_Bash_History | grep -c "Joe Germuska"
	2
cat AAA Delta_SkyMiles Terminal_City_Library Museum_of_Bash_History | grep -c "Jeremy Bowers"
	4

cd ..
grep "Jeremy Bowers" people
head -n 284 streets/Dunstable_Road | tail -n 1
	SEE INTERVIEW #9620713
cat interviews/interview-9620713
	Home appears to be empty, no answer at the door.
	After questioning neighbors, appears that the occupant may have left for a trip recently. Considered a suspect until proven otherwise, but would have to eliminate other suspects to confirm.

grep "Joe Germuska" people
head -n 275 streets/Plainfield_Street | tail -n 1
	SEE INTERVIEW #29741223
cat interviews/interview-29741223
	Should not be considered a suspect, has no SkyMiles membership and has never been a member of the Museum of Bash History.

Jeremy Bowers is the killer.