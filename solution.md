cd mystery
cat instructions
cd mystery
cat crimescene
grep 'CLUE' crimescene
grep 'Annabel' people
cd streets
ls
cat Hart_Place
cd ..
cd memberships
cat AAA
ls
grep 'Annabel' AAA

Pulled only 'Annabel' from list of people and AAA memberships as
'Annabel Church'

grep 'Annabel' Delta_SkyMiles

No Annabel in DSM

cd ..

grep 'Annabel' Terminal_City_Library

No Annabel in TCL

grep 'Annabel' Museum_of_Bash_History

Two Annabels returned
'Annabel Church' and 'Oluwasegun Annabel'

cd ..

cat vehicles
grep 'Annabel' vehicles

Four Annabels returned
'Oluwasegun Annabel', 'Annabel Church', 'Annabel Sun', 'Annabel Fuglsang'

cat people
grep 'Annabel' people

returned Annabel Sun	F	26	Hart Place, line 40
Oluwasegun Annabel	M	37	Mattapan Street, line 173
Annabel Church	F	38	Buckingham Place, line 179
Annabel Fuglsang	M	40	Haley Street, line 176

cd streets
ls
cat Buckingham_Place
head -n179 Buckingham_Place

got 'SEE INTERVIEW #699607'

cd ..
cd interviews
cat interview-699607

Ms. Annabel Church reports car fled scene was blue honda 
with license beginning with "L337" and ending with "9"

cd ..
grep 'L337' vehicles

grep -A 5 'L337' vehicles

Two match description of suspect as owning BLUE HONDA 
with license plate beginning 'L337' and ending '9'
who are Male and 6'

"Joe Germuska" and "Jeremy Bowers"

grep 'Jeremy Bowers' people
Jeremy Bowers	M	34	Dunstable Road, line 284

grep 'Joe Germuska' people
Joe Germuska	M	65	Plainfield Street, line 275

cd streets
head -n284 Dunstable_Road
returned 'SEE INTERVIEW #9620713'

cd interviews
cat interview-9620713 Jeremy
No one home, may have left for trip as per suggestion of neightbor, 
must eliminate other suspects

cd ..

cd streets
head -n275 Plainsfield_Street
returned 'SEE INTERVIEW #29741223'

cd ..
cd interviews

cat interview-29741223 Joe
No Memberships to SkyMiles or Museum of Bash History

cd ..
grep -r "Bowers" memberships
returns
memberships/AAA:Jeremy Bowers
memberships/Delta_SkyMiles:Jeremy Bowers
memberships/Museum_of_Bash_History:Jeremy Bowers
memberships/Terminal_City_Library:Jeremy Bowers
These match all cards in wallet

Jeremy Bowers matches all suspect description in clues.

JEREMY BOWERS IS THE CULPRIT