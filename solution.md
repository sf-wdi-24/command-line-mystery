Dave Sloan

Trung and I did it together so here is his version since its cleaner.  My version had 16000 lines. 

Last login: Mon Oct 26 14:39:20 on ttys000
➜  ~  cd develop
➜  develop  cd command-line-mystery
➜  command-line-mystery git:(master) cat instructions
.OOOOOOOOOOOOOOO @@                                   @@ OOOOOOOOOOOOOOOO.
OOOOOOOOOOOOOOOO @@                                    @@ OOOOOOOOOOOOOOOO
OOOOOOOOOO'''''' @@                                    @@ ```````OOOOOOOOO
OOOOO'' aaa@@@@@@@@@@@@@@@@@@@@"""                   """""""""@@aaaa `OOOO
OOOOO,""""@@@@@@@@@@@@@@""""                                     a@"" OOOA
OOOOOOOOOoooooo,                                            |OOoooooOOOOOS
OOOOOOOOOOOOOOOOo,                                          |OOOOOOOOOOOOC
OOOOOOOOOOOOOOOOOO                                         ,|OOOOOOOOOOOOI
OOOOOOOOOOOOOOOOOO @          THE                          |OOOOOOOOOOOOOI
OOOOOOOOOOOOOOOOO'@           COMMAND                      OOOOOOOOOOOOOOb
OOOOOOOOOOOOOOO'a'            LINE                         |OOOOOOOOOOOOOy
OOOOOOOOOOOOOO''              MURDERS                      aa`OOOOOOOOOOOP
OOOOOOOOOOOOOOb,..                                          `@aa``OOOOOOOh
OOOOOOOOOOOOOOOOOOo                                           `@@@aa OOOOo
OOOOOOOOOOOOOOOOOOO|                                             @@@ OOOOe
OOOOOOOOOOOOOOOOOOO@                               aaaaaaa       @@',OOOOn
OOOOOOOOOOOOOOOOOOO@                        aaa@@@@@@@@""        @@ OOOOOi
OOOOOOOOOO~~ aaaaaa"a                 aaa@@@@@@@@@@""            @@ OOOOOx
OOOOOO aaaa@"""""""" ""            @@@@@@@@@@@@""               @@@|`OOOO'
OOOOOOOo`@@a                  aa@@  @@@@@@@""         a@        @@@@ OOOO9
OOOOOOO'  `@@a               @@a@@   @@""           a@@   a     |@@@ OOOO3
`OOOO'       `@    aa@@       aaa"""          @a        a@     a@@@',OOOO'


There's been a murder in Terminal City, and TCPD needs your help.

To figure out whodunit, go to the "mystery" sub-directory and start working from there.

You'll want to start by collecting all the clues at the crime scene (the "crimescene" file).

The officers on the scene are pretty meticulous, so they've written down EVERYTHING in their officer reports.

Fortunately the sergeant went through and marked the real clues with the word "CLUE" in all caps.

If you get stuck, open one of the hint files (from the Command Line, type "cat hint1", "cat hint2", etc.).

For tips on getting started with the Command Line, open "cheatsheet.md".

Don't use a text editor to view any files except "readme.md" and "cheatsheet.md".
➜  command-line-mystery git:(master) ls
cheatsheet.md hint1         hint2         hint3         hint4         hint5         hint6         hint7         hint8         instructions  mystery       readme.md
➜  command-line-mystery git:(master) cat hint1
Try poking around what's in a file by using the 'head' command:

  head -n 20 people

This will show you the first 20 lines of the 'people' file.%                                                                                                                         ➜  command-line-mystery git:(master) head -n 20 people
head: people: No such file or directory
➜  command-line-mystery git:(master) head -n 20 mystery/people
***************
To go to the street someone lives on, use the file
for that street name in the 'streets' subdirectory.
To knock on their door and investigate, read the line number
they live on from the file.  If a line looks like gibberish, you're at the wrong house.
***************

NAME	GENDER	AGE	ADDRESS
Alicia Fuentes	F	48	Walton Street, line 433
Jo-Ting Losev	F	46	Hemenway Street, line 390
Elena Edmonds	F	58	Elmwood Avenue, line 123
Naydene Cabral	F	46	Winthrop Street, line 454
Dato Rosengren	M	22	Mystic Street, line 477
Fernanda Serrano	F	37	Redlands Road, line 392
Emiliano Wenk	M	90	Paulding Street, line 490
Larry Lapin	M	71	Atwill Road, line 298
Jakub Gondos	M	61	Mitchell Street, line 187
Derek Kazanin	M	55	Tennis Road, line 440
Jens Tuimalealiifano	M	83	Rockwood Street, line 205
Nikola Kadhi	M	75	Glenville Avenue, line 226
➜  command-line-mystery git:(master) ls mistery/streets
ls: mistery/streets: No such file or directory
➜  command-line-mystery git:(master) cd mistery
cd: no such file or directory: mistery
➜  command-line-mystery git:(master) ls mystery/streets
Abbot_Street             Brookline_Avenue         Embassy_Road             High_View_Avenue         Merola_Park              Randlett_Place           Theodore_Street
Acton_Street             Buckingham_Place         Enterprise_Street        Hobart_Street            Michigan_Avenue          Rena_Street              Tolman_Street
Addington_Road           Burwell_Road             Esther_Road              Hollander_Street         Miles_Street             Renfrew_Street           Topeka_Street
Alaric_Street            Cadbury_Road             Estrella_Street          Hooten_Court             Moloney_Street           Richard_Avenue           Trapelo_Street
Albany_Street            Cardinal_Medeiros_Avenue Eugenia_Road             Hopedale_Street          Mount_Ash_Road           Richardson_Street        Trident_Street
Aldworth_Street          Cardington_Street        Fairfield_Street         Hull_Street              Mount_Ida_Road           Richmond_Street          Trinity_Place
Alpine_Street            Causeway_Street          Faunce_Road              Island_View_Place        Mountain_Avenue          River_Street             Unity_Court
Andover_Road             Cerdan_Avenue            Fay_Street               Jacob_Street             Mozart_Street            Rivermoor_Street         Vassal_Lane
Ansonia_Road             Channel_Center_Street    Fayston_Street           Jacqueline_Road          Myles_Standish_Road      Rockmere_Street          Victory_Road
Appleton_Road            Cheverus_Road            Fessenden_Street         Jamaica_Place            Mystic_Street            Rosaria_Street           Vinton_Street
Aramon_Street            Claremont_Park           Forestvale_Road          Jersey_Street            Nazing_Street            Rowe_Street              Vista_Street
Arcola_Street            Clay_Street              Foundry_Street           Jeshurun_Street          New_Minton_Street        Rozella_Street           Waldeck_Street
Atwood_Road              Claybourne_Street        Fowler_Street            John_Alden_Road          New_Park_Avenue          Saco_Street              Wallingford_Road
Auriga_Street            Clipper_Ship_Lane        Frontage_Road            Judge_Street             Newcastle_Road           Saint_Saveur_Court       Warren_Avenue
Avalon_Road              Cook_Street              Gerard_Street            June_Street              Newcroft_Circle          Salutation_Street        Wentworth_Street
B_Street                 Cornelia_Street          Gillespies_Lane          Kearsarge_Avenue         North_Washington_Street  Sammett_Avenue           Wesley_Place
Ballard_Street           Corwin_Street            Glenville_Avenue         King_Place               Norton_Street            Saunders_Street          Wheatland_Avenue
Balmoral_Park            Culbert_Street           Glenwood_Avenue          Kinross_Road             Oak_Hill_Avenue          Scotia_Street            Wiget_Street
Bartlett_Avenue          Dacia_Street             Grampian_Way             Knoll_Street             Oak_Place                Searle_Road              Wiggin_Street
Bellevue_Avenue          Dalton_Street            Granby_Street            Laban_Pratt_Road         Oakley_Street            Selwyn_Street            Wilcox_Road
Bertson_Avenue           Dana_Avenue              Gray_Gardens_East        Leseur_Road              Oliva_Road               Senders_Court            Wilkinson_Park
Bicknell_Street          Davenport_Street         Greendale_Road           Lineham_Court            Orchard_Road             Sheldon_Street           Willet_Street
Blue_Hill_Avenue         Devine_Way               Gretter_Road             Lovis_Street             Paragon_Road             Silver_Street            Williston_Road
Bobolink_Street          Dewar_Street             Groveland_Street         Lynde_Street             Peacock_Lane             Sparrow_Street           Willowdean_Avenue
Boston_Street            Doane_Street             Hadassah_Way             Lynn_Street              Peter_Parley_Road        Spaulding_Street         Wilmington_Avenue
Bothwell_Road            Dock_Street              Haley_Street             Mamelon_Circle           Pinewood_Street          Standard_Street          Winter_Street
Bournedale_Road          Dorrance_Street          Harbor_Point_Boulevard   Manila_Avenue            Plain_Street             Staniford_Street         Woodcliff_Street
Boynton_Street           Dover_Street             Harding_Road             Manton_Terrace           Plainfield_Street        Story_Street             Wooddale_Avenue
Brinton_Street           Dresser_Street           Hart_Place               Marney_Street            Potosi_Street            Supple_Road              Worrell_Street
Bristol_Street           Drumlin_Road             Hazel_Street             Mattapan_Street          Priscilla_Road           Taunton_Avenue           Wycliff_Avenue
Broad_Canal_Street       Dunstable_Road           Hazelton_Street          May_Street               Proctor_Street           Tennyson_Street
Brookdale_Street         Elmore_Street            High_Road                Meadowview_Road          Quarley_Road             Terrace_Place
➜  command-line-mystery git:(master) cat hint2
Try using grep to search for the clues in the crimescene file:

	grep "CLUE" crimescene%                                                                                                                                                      ➜  command-line-mystery git:(master) grep "CLUE" crimescene
grep: crimescene: No such file or directory
➜  command-line-mystery git:(master) grep "CLUE" mystery/crimescene
CLUE: Footage from an ATM security camera is blurry but shows that the perpetrator is a tall male, at least 6'.
CLUE: Found a wallet believed to belong to the killer: no ID, just loose change, and membership cards for AAA, Delta SkyMiles, the local library, and the Museum of Bash History. The cards are totally untraceable and have no name, for some reason.
CLUE: Questioned the barista at the local coffee shop. He said a woman left right before they heard the shots. The name on her latte was Annabel, she had blond spiky hair and a New Zealand accent.
➜  command-line-mystery git:(master) cat hint3
In order to track down our potential witness, we need to figure out where she lives.

Try using 'head' on some of the files like 'people' and 'vehicles' and see where we might find that.%                                                                                ➜  command-line-mystery git:(master) head -n 10 vehicles
head: vehicles: No such file or directory
➜  command-line-mystery git:(master) head -n 10 mystery/vehicles
***************
Vehicle and owner information from the Terminal City Department of Motor Vehicles
***************

License Plate T3YUHF6
Make: Toyota
Color: Yellow
Owner: Jianbo Megannem
Height: 5'6"
Weight: 246 lbs
➜  command-line-mystery git:(master) cat hint 4
cat: hint: No such file or directory
cat: 4: No such file or directory
➜  command-line-mystery git:(master) cat hint4 
To find all the Annabels' addresses, use the 'people' file:

	grep "Annabel" people

Notice that not all of the results are worth investigating.  Remember what we know about Annabel.%                                                                                   ➜  command-line-mystery git:(master) grep "Annabel" people
grep: people: No such file or directory
➜  command-line-mystery git:(master) grep "Annabel" mystery/people
Annabel Sun	F	26	Hart Place, line 40
Oluwasegun Annabel	M	37	Mattapan Street, line 173
Annabel Church	F	38	Buckingham Place, line 179
Annabel Fuglsang	M	40	Haley Street, line 176
➜  command-line-mystery git:(master) head -40 mystery/streets/Hart_Place
downhills exaggerates outgo rebating rhyming militarizes 
rakishly lithographs inserts 
humanism revolt hoggish tuner hoofs frizziest 
strippers toady framers bakes mandate 
pear graver drubbing reinvest abnormality teetotal lend 
stipulate attiring sprint tunnelings sera merrily proofreaders 
enthroning tuber onrushes pat a rows degrades parleyed 
probationer irresponsibility spongier smirking diminished 
stipulations dandle repetitious enervate 
reunion insert unhand heartbeat busheling teakettles dismayed 
plug hates easiest jabbered destining agglutinates 
ambitious swaggering ties annoyed battleground 
intuitively humbugs ribaldry suspend 
bedspreads expansionists restfullest 
dilated outstrips teapot fluoridates shops mammoth 
baron zoos teeter falloffs fishes invalidating 
patrols knelling rosining lightness unburden 
surfeited absurdity plexus rebuses leaking standing 
sizable punter bagginess dissenters 
postmarking spades overdraft pointillism 
stymie treadles extortionists dietitians agonies spitefuller 
multiplied submits despotism adventurous ballsier 
parody mania leftism tranquilize sexpots stupor parleying 
triumphing whiskered razing danger preordains 
faker preparatory gabbing mavens vamped 
idles tents oratorios butternuts upholsterers sassafras 
damnedest apologists inveigh 
propriety tossed parallelling town kinkier quarantine 
oxymoron nonmembers taproots 
snakebite dramatizing dawdling enlightening 
swastikas fragrant voluble stowing 
grammarian shah ambushed alines varmints doze detains 
wondrous uphold tests appetites wilier beautifiers 
drifts dosages leprosy rashers badmouth jugglers 
snot appals primes whet annular tonality 
shivery kingdom supplements envying 
the slayer gesture waged twenties ratifying baling mortals 
doggie probationary demurer fatness 
stupendous prolonged smog naps 
SEE INTERVIEW #47246024
➜  command-line-mystery git:(master) cat mystery/interviews/interview-47246024
Ms. Sun has brown hair and is not from New Zealand.  Not the witness from the cafe.%                                                                                                 ➜  command-line-mystery git:(master) head -40 mystery/streets/Buckingham_Place
one earthlings startles invitingly pall 
headwaiter mate impregnability 
unmake drainpipe utilities pointillist 
apropos impressively forborne finite exempt 
griming vised thankfully burlap hypertension 
landsliding landfill furlong mittens heartland 
bully tortoise enlargers roamed undressing 
yuks troubleshooting seaboards 
springtime deaves reinitialize puttying 
densities warranties penultimates dehumanizes perorations 
untangles stays smashing spinets breadfruits 
granulating toreadors finishes knob headhunter 
longhairs pennyweights womanizers 
depressive overused disturbs glandular pillowed 
fallibly proportioning settling jumpier 
vagueness lethal alienating potted 
immortalizing parfaits ignited malnutrition 
feisty senseless manly fifths tailspin supposed downstairs 
ringer drainers agiler pinholes reedier 
meekest revolvers gobblers panelists unassigned yew butterfly 
nuts singsonged writs arm dimness 
bearing shags kleptomania sprinted barkers 
augury bullied letups shimming filmy golds 
thunders forbid snowflake unstabler moralist 
torrential attributable poniards newsletter stealthier 
breastplates bundled nationalization 
invaliding fitfully figured keystones 
misdoing unplugged newspapermen grandstand 
shrouding pushed botanists pivots domed 
mealier formerly trivet avenues flukey humorously 
twofold sniffling misdoes intros bookmarked 
subordinated amateur ambition tarpons fluttery 
gassier soldiering irritant wavelengths wriggling 
tarots gruesomely pair minks enrapture 
stupefy dukedoms emanating manikin enshrines 
freaky meditated paginating suddenly farewells presentations 
darted sizes tartly meddlers startled 
strong love thumbnail aquifer samurai 
parleys mobilizing repertoires sanitarium punts 
entwining inkier exterminate remission purblind 
➜  command-line-mystery git:(master) head -179 mystery/streets/Buckingham_Place
one earthlings startles invitingly pall 
headwaiter mate impregnability 
unmake drainpipe utilities pointillist 
apropos impressively forborne finite exempt 
griming vised thankfully burlap hypertension 
landsliding landfill furlong mittens heartland 
bully tortoise enlargers roamed undressing 
yuks troubleshooting seaboards 
springtime deaves reinitialize puttying 
densities warranties penultimates dehumanizes perorations 
untangles stays smashing spinets breadfruits 
granulating toreadors finishes knob headhunter 
longhairs pennyweights womanizers 
depressive overused disturbs glandular pillowed 
fallibly proportioning settling jumpier 
vagueness lethal alienating potted 
immortalizing parfaits ignited malnutrition 
feisty senseless manly fifths tailspin supposed downstairs 
ringer drainers agiler pinholes reedier 
meekest revolvers gobblers panelists unassigned yew butterfly 
nuts singsonged writs arm dimness 
bearing shags kleptomania sprinted barkers 
augury bullied letups shimming filmy golds 
thunders forbid snowflake unstabler moralist 
torrential attributable poniards newsletter stealthier 
breastplates bundled nationalization 
invaliding fitfully figured keystones 
misdoing unplugged newspapermen grandstand 
shrouding pushed botanists pivots domed 
mealier formerly trivet avenues flukey humorously 
twofold sniffling misdoes intros bookmarked 
subordinated amateur ambition tarpons fluttery 
gassier soldiering irritant wavelengths wriggling 
tarots gruesomely pair minks enrapture 
stupefy dukedoms emanating manikin enshrines 
freaky meditated paginating suddenly farewells presentations 
darted sizes tartly meddlers startled 
strong love thumbnail aquifer samurai 
parleys mobilizing repertoires sanitarium punts 
entwining inkier exterminate remission purblind 
inflammations resist impedes lighthouses allegro 
additions pantomiming wrongdoing natives elusive opals 
finagles assaying raving primmest libel repairable 
gallbladders dismissed girders waxworks tenderly feasibly 
temporaries peephole whams faultfinding metabolizing 
floor huddles refinish flattering swamped 
levied whets undersign bestiary 
auras kite presumes toasty pair loping revelled teas abnormally 
reality polarized preferably nominated 
pawnshops bootie pealed violist haulers haled 
palmettoes waste spot soggier annulled 
steak shrews gunshots foregone kneel 
inlets bran maraud salts hemmed 
poniard mangled dither humblest demitasses proprietary 
augury telemetry starlit landlubbers 
portrayed battleships orderliness salver forming grits 
alleyways disowning blogged argosies 
supervisor adored unequalled dangle nonreturnables 
sixteens defaulted bandoliers turtledove 
gearwheels junks endlessly wear internship timidly maxim 
waver windbreaker sunken disguising importations 
shoots smoggiest lifestyles journeymen 
reffed raft futzing dagger surrealism 
unsupervised disrepute ingeniously annul divining 
expressing rib snorted hexagons sway sharing neurosurgery 
frazzled leaving aqueous stigma punning psalmists 
desirous devaluation pudding alight squealed 
marital unsubstantial peasant drying bee agglomerates 
hansom methought adapts muezzins relish 
eastward maydays gondola burger abstains predetermined gated 
ornithology unarmed godfather roomer penises primitives 
slumber ether mender edgy underhanded ablest affirmatively 
sex barbershops leotards bobolink hormonal sump 
indubitable yardages felons unquestionably versifies infinitesimals 
aliasing inhibiting originally synthesizes 
perjuries goblet pasta moves farrow urged dotes fluffs 
liberals indentation horns erosion harrow snowstorm emulator 
pretending expiation imperialist overdresses 
bookmakers analogues dittoed effigy thunderheads 
employee wafer pessimist alleyway envisages 
orderings bedbug employ muskmelon benumb 
shards ominous bawl worryings refills animators soften 
merrier vanadium provides medleys obstinately summoner 
fold swoons grievously dismantles 
unbroken hothead jessamine yolk loath rake 
bludgeoned inflationary dowdy fingers saunter 
great diminutive puffiness bankbooks 
insolvent more balms millions mommy river sullenest 
intertwines obeisant gallon blame tub seeking firsts 
lingered populates naughty galvanizes postulated 
frailest shin wrestle faking goddamed allergist minute lobotomies 
thrower industriously idolized unabashed understudied 
shaking refereed mullet harmfulness hasp 
tubeless irretrievable transits underwrites drainage 
renegaded bilk gearbox expertise away beating 
rapt preventative freedman trouts insulted peopling pales 
earnest blabbing prohibitionist deserts runway 
patents idiot marvel deadens shad sluggers essay talkative 
sneer lows sidled sparingly ink geranium lighthearted 
boudoirs merry juniper while liquifies phobias goad peanuts 
hesitating inverse nighttime 
loosely impish threaded formlessness signet 
knotted pursues sightseer history software 
admonishment underskirt speedway deviate fags 
sandblasting plodding faggots grungy eventuality 
workmen extemporaneous espouses straitening laxatives 
harangue summing binderies membership 
huskies sidesaddles restoration tawdriest gazillions 
liven delimit jibe profited butterfly faithful 
iodize wheezier ministration hotbed rehabbing nuzzle 
esquire swallows smelly grounder shimmering sharpers hexed 
legionnaires workdays rinds personality 
governor floury earrings overusing 
winsomer falsity paradigm rows wiry alas worship 
spears goaded took despaired betrothal mink doled penetrative 
ingot tasting uprights barks sottish troubleshooter 
persevere ping deafening kisser innovators 
gaudier noiselessly glamorously quasar beeping yesterdays 
spinal klutzes yeastier initializing 
foetuses brews blunderbuss emitting 
hillier streak opines retirement straightedges nontransferable 
mending envisions gizmos drags finnier wildest 
adder malingerers euphony antiphonal departs spitfires 
hypes dye illuminations disablement 
sender waned bottomless saintlier lades plethora 
shenanigan larynges penguin heatstroke 
steins exiles underestimating guts billet flabbergasting 
sieges flawlessly serialized kippers 
enfeeble weathered bedridden liquidations 
flints winners unfairest damaged 
partnered pilaws hogs pluming avenge 
tanker forwent sag pheromone snowdrifts syphons 
mimes mountaineers exalted disfigure shelves nimble 
flusters derivable potato establishment 
regimen betterment sarape misused balladeer pilling 
besiegers whitens dinky stupid 
kettle borax partnering preppiest 
fisherman dappling mustier fobs figuratively orthopaedists 
jumpiest tundra hybridizing 
inexhaustibly thrower metaphors intones slanted 
insinuated garrison prettifying attests 
stemming shrewdness prigs workweek feebleness abiding distrust 
sternest rowel debater peas adversely enshrouds 
premiss nowhere billion gatherings fetid traded 
misappropriation donations printers 
dethronement holler spurned divisors 
reverts plaza obsequiously permutation 
grandpas tyrants metastases personae hauler eyelash 
outrage shelters soured surlier metronome moonlighted 
mailmen maneuverable mattered seeding dehumanizes 
spiniest dents weightless kookaburras misprinted disorders 
intermediary selling jersey polymaths empathizing 
doubling peaked owlish byline levitates suspense relabels 
autumns wiping dhotis damming twentieth proportion 
potentate bribes rifer moderate verbena desire framing 
twaddle polite pretext mazourka situated 
bilking darling tempera stresses earmarking 
breezes fretted exhumed fertile 
vineyards gingerbread ridgepoles helixes 
deal heppest malignantly tallest ebony 
flexible espressos prioresses linoleum deposed tourism 
sophomore filtering prostitute wasps 
parboiling sine rain unprofessional 
surrey mudslide brilliants planing derail wilder 
environmentally professor frenzies trolled 
watermelons garrisoning imprisonments typified 
busied besetting founders flurried state trill 
hyphened flashiest advertise byline patrons fighter goldsmith 
sightread teazles footfall washbasin molesting 
grainiest lobbing shrouded largest jump geometries 
eluded sophism stages pertly sewerage biplanes maturer travelogs 
fords plaque droned spars misleading sunburn 
serenely shits dialyses roistering registrars pointillists 
bales napes warts mammary referrals fisherman training 
panting battalion greedier allergens orotund 
headers badge bullhorn agglutinating bearable 
analogs departing anguished nylons 
whitewall napkins overheats embittering grimmer beamed 
SEE INTERVIEW #699607
➜  command-line-mystery git:(master) cat mystery/interviews/interview-699607  
Interviewed Ms. Church at 2:04 pm.  Witness stated that she did not see anyone she could identify as the shooter, that she ran away as soon as the shots were fired.

However, she reports seeing the car that fled the scene.  Describes it as a blue Honda, with a license plate that starts with "L337" and ends with "9"%                              ➜  command-line-mystery git:(master) cat hint5
"Interview" the two possible witnesses by reading the correct line from the streets they live on:

	head -n 173 streets/Mattapan_Street | tail -n 1

This will give you just line 173 of Mattapan street, because it will take first 173 lines, and then take
the last line from those.%                                                                                                                                                           ➜  command-line-mystery git:(master) cat hint6
To find a matching license plate, or a matching car, you can use grep on the 'vehicles' file:

	grep "Honda" vehicles

	grep "Blue" vehicles

	grep "L337" vehicles

This doesn't give us anything useful - why not? Try using 'head' on the file to investigate its structure.%                                                                          ➜  command-line-mystery git:(master) grep -A 7 "L337" mystery/vehicles
License Plate L337ZR9
Make: Honda
Color: Red
Owner: Katie Park
Height: 6'2"
Weight: 189 lbs

License Plate FF9UF7C
--
License Plate L337P89
Make: Honda
Color: Teal
Owner: Mike Bostock
Height: 6'4"
Weight: 173 lbs

License Plate JBGQDXM
--
License Plate L337GX9
Make: Mazda
Color: Orange
Owner: John Keefe
Height: 6'4"
Weight: 185 lbs

License Plate F3TYJET
--
License Plate L337QE9
Make: Honda
Color: Blue
Owner: Erika Owens
Height: 6'5"
Weight: 220 lbs

License Plate 3PODXFM
--
License Plate L337GB9
Make: Toyota
Color: Blue
Owner: Matt Waite
Height: 6'1"
Weight: 190 lbs

License Plate UK8RV00
--
License Plate L337OI9
Make: Jaguar
Color: Blue
Owner: Brian Boyer
Height: 6'6"
Weight: 201 lbs

License Plate JFIUVDB
--
License Plate L337X19
Make: Fiat
Color: Blue
Owner: Al Shaw
Height: 6'5"
Weight: 240 lbs

License Plate SP0817V
--
License Plate L337539
Make: Honda
Color: Blue
Owner: Aron Pilhofer
Height: 5'3"
Weight: 198 lbs

License Plate 8C5LC5N
--
License Plate L3373U9
Make: Ford
Color: Blue
Owner: Miranda Mulligan
Height: 6'6"
Weight: 156 lbs

License Plate XDI2UCE
--
License Plate L337369
Make: Honda
Color: Blue
Owner: Heather Billings
Height: 5'2"
Weight: 244 lbs

License Plate HYPVZ7R
--
License Plate L337DV9
Make: Honda
Color: Blue
Owner: Joe Germuska
Height: 6'2"
Weight: 164 lbs

License Plate G9J35EZ
--
License Plate L3375A9
Make: Honda
Color: Blue
Owner: Jeremy Bowers
Height: 6'1"
Weight: 204 lbs

License Plate SEZHWM5
--
License Plate L337WR9
Make: Honda
Color: Blue
Owner: Jacqui Maher
Height: 6'2"
Weight: 130 lbs

License Plate 1FEDUD0
➜  command-line-mystery git:(master) grep -A 5 "L337" mystery/vehicles
License Plate L337ZR9
Make: Honda
Color: Red
Owner: Katie Park
Height: 6'2"
Weight: 189 lbs
--
License Plate L337P89
Make: Honda
Color: Teal
Owner: Mike Bostock
Height: 6'4"
Weight: 173 lbs
--
License Plate L337GX9
Make: Mazda
Color: Orange
Owner: John Keefe
Height: 6'4"
Weight: 185 lbs
--
License Plate L337QE9
Make: Honda
Color: Blue
Owner: Erika Owens
Height: 6'5"
Weight: 220 lbs
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
License Plate L337X19
Make: Fiat
Color: Blue
Owner: Al Shaw
Height: 6'5"
Weight: 240 lbs
--
License Plate L337539
Make: Honda
Color: Blue
Owner: Aron Pilhofer
Height: 5'3"
Weight: 198 lbs
--
License Plate L3373U9
Make: Ford
Color: Blue
Owner: Miranda Mulligan
Height: 6'6"
Weight: 156 lbs
--
License Plate L337369
Make: Honda
Color: Blue
Owner: Heather Billings
Height: 5'2"
Weight: 244 lbs
--
License Plate L337DV9
Make: Honda
Color: Blue
Owner: Joe Germuska
Height: 6'2"
Weight: 164 lbs
--
License Plate L3375A9
Make: Honda
Color: Blue
Owner: Jeremy Bowers
Height: 6'1"
Weight: 204 lbs
--
License Plate L337WR9
Make: Honda
Color: Blue
Owner: Jacqui Maher
Height: 6'2"
Weight: 130 lbs
➜  command-line-mystery git:(master) grep -R "Jacqui Maher" mystery/memberships
mystery/memberships/AAA:Jacqui Maher
mystery/memberships/Delta_SkyMiles:Jacqui Maher
mystery/memberships/Museum_of_Bash_History:Jacqui Maher
mystery/memberships/Terminal_City_Library:Jacqui Maher
➜  command-line-mystery git:(master) grep "Jacqui Maher" mystery/people      
Jacqui Maher	F	40	Andover Road, line 224
➜  command-line-mystery git:(master) 

Jeremy Bowers did it!  He is the only male that drives a honda that is blue and is a member of all four clubs. 

