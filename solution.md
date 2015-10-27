navigating to thr directory:

cd develop 
cd command-line-mystery
ls

display the instructions:

cat instructions

searchinh for "CLUE" in the mystery dir:

grep -r "CLUE" mystery //got 3 clues 

navigate to the mystery dir to chck the directories and files under it:

cd mystery

navigate into all the directories in mystery to check the content:

cd  interviews
cd ..
cd memberships
cd ..
cd  streets
cd ..


search for Annabel in people:

grep "Annabel" people // found 2 females

open the street file:

cd streets
ls

copy the street name as it's displayed in the file and open the street name and the file with the line num as it discribed in the people file (1 time with line 40 and secund with line 179):

head -n40 Hart_Place // refered to inteview #47246024

head -n179 Buckingham_Place // refered to inteview #699607

going back to the interviews:
 cd ..
 cd interviews

 open the interviews:

 open interview-47246024 // not the right Annabel

 open interview-699607 // found that Annabel Church is the right woman from the cafe. the killer dove a blue Honda, with a license plate that starts with "L337" and ends with "9"

search for "L337" under vehicles:

grep -A 5 "L337" vehicles // found 3 people witha male name over 6" and with blue honda. (Joe Germuska, Jeremy Bowers, Jacqui Maher)

check all the 3 names in people to verify sex is male:

grep "Joe Germuska" people // is a male

grep "Jeremy Bowers" people // is a male

grep "Jacqui Maher" people // is a female

checking who has AAA club:

cd memberships

grep "Jeremy Bowers" AAA //has AAA
grep "Joe Germuska" AAA  // has AAA

checking who has  Delta_SkyMiles:

grep "Joe Germuska"  Delta_SkyMiles //doesn't has
grep "Jeremy Bowers"  Delta_SkyMiles //has Delta_SkyMiles


The Killer is Jeremy Bowers!!!!!!


















