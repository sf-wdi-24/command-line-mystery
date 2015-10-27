
## Jeremy Bowers is the murderer
---------------------------------
List of Terminal Commands needed to Solve
---------------------------------
Aquire Clues
1. grep "CLUE" crimescene (Aquire Clues)
2. grep "Annabel" people (Find people with name of Annabel)
3. cd /Users/rockway/develop/command-line-mystery/mystery/streets
4. head -n 40 Hart_Place | tail -n 1 (Search based on Annabel addresses)
5. head -n 179 Buckingham_Place | tail -n 1 (Search based on Annabel addresses)
6. cd /Users/rockway/develop/command-line-mystery/mystery/interviews
7. cat interview-47246024 (Search based on Address info)
8. cat interview-699607 (Search based on Address info)
9. cd /Users/rockway/develop/command-line-mystery/mystery
10. grep -A 6 "L337" vehicles | grep -A 6 "Honda" | grep -A 6 "Blue" (Search for a Blue Honda with L337)
11. cd /Users/rockway/develop/command-line-mystery/mystery/memberships
12. cat AAA Delta_SkyMiles Terminal_City_Library Museum_of_Bash_History | grep "Jeremy Bowers" (Search to see if name has memberships in all)
13. cat AAA Delta_SkyMiles Terminal_City_Library Museum_of_Bash_History | grep "Joe Germuska" (Search to see if name has memberships in all)