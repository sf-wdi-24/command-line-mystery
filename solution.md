grep "Clue" crimescene 		/* 1. This is done while in the Mystery/ directory. Returns 3 clues: 
							a. Is a tall, at least 6ft., male according to video footage. 
							b. Found a wallet believed to be the killer with untraceable membership cards to: AAA, Delta Sky, local library, and Museum of BASH history.
							c. Possible witness: "Annabel", a barista, New Zealand accent, blonde hair*/


grep "Annabel" people 		/*2. This is to find the witness' actual name...the clue's given info is shakey. 
							There are multiple names containing Annabel. Searched for them in Witnesses by their other given name other than Annabel.
							One Annabell, "Church" is most appropriate*/					


grep "Church" * 			/*3. This is done while in the Interviews directory. Returns "Interview-689607". 
							Reports "seeing" the shooter fleeding in a blue Honda, with plate numbers beginning w/ "L337" and ending in "9". */


grep -A 5 "L337" *			/*4A. This is done in the vehicles directory. Got help from catenating hint7...was having troubles figuring out how to read the Vehicle file.
							Did this suggested code (searches for "L337" in the Vehicles file, and for all the matches, it catenates the result along with the
							following 5 lines). Upon reading the results, and cross checking the names in the Members directory, */

grep "Jeremy" *				/*4B. Did this in Members directory to cross check with the appropriate names that the grep on the lisc. plate number returned.
							A Mr. "Jeremy Bowers" seems to be the best possible answer, I think, and therefore is my shooter. He is: 
							a. tall
							b. a member of all 3 clubs that were found in the wallet at the crimescen
							c. has no return in the Interviews directoy when searched for him
							So, he is my shooter? */							
