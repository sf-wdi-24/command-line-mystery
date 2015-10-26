➜  command-line-mystery git:(master) ✗ cat instructions
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
<br>
➜  command-line-mystery git:(master) cd mystery
<br>
➜  mystery git:(master) ✗ grep -R "CLUE" ./
.//crimescene:CLUE: Footage from an ATM security camera is blurry but shows that the perpetrator is a tall male, at least 6'.
.//crimescene:CLUE: Found a wallet believed to belong to the killer: no ID, just loose change, and membership cards for AAA, Delta SkyMiles, the local library, and the Museum of Bash History. The cards are totally untraceable and have no name, for some reason.
.//crimescene:CLUE: Questioned the barista at the local coffee shop. He said a woman left right before they heard the shots. The name on her latte was Annabel, she had blond spiky hair and a New Zealand accent.
<br>
➜  mystery git:(master) grep -R "Annabel" people
people:Annabel Sun	F	26	Hart Place, line 40
people:Oluwasegun Annabel	M	37	Mattapan Street, line 173
people:Annabel Church	F	38	Buckingham Place, line 179
people:Annabel Fuglsang	M	40	Haley Street, line 176
<br>
➜  mystery git:(master) ✗ grep -R "Hart Place" people
people:Remy Barac	M	77	Hart Place, line 492
people:Denis Rezola	M	24	Hart Place, line 405
people:Annabel Sun	F	26	Hart Place, line 40
people:Nahla Zhedik	F	32	Hart Place, line 349
➜  mystery git:(master) ✗ grep -R "Mattapan Street" people
people:Oluwasegun Annabel	M	37	Mattapan Street, line 173
people:Francisco Lips	M	71	Mattapan Street, line 295
➜  mystery git:(master) ✗ grep -R "Buckingham Place" people
people:Annabel Church	F	38	Buckingham Place, line 179
➜  mystery git:(master) ✗ grep -R "Haley Street" people    
**people:Annabel Fuglsang	M	40	Haley Street, line 176
people:Ahmed Chammartin	M	22	Haley Street, line 301
<br>
➜  mystery git:(master) ✗ grep -R "Remy Barac" vehicles -3
vehicles-License Plate ZKP6TJH
vehicles-Make: Fiat
vehicles-Color: Red
vehicles:Owner: Remy Barac
vehicles-Height: 6'4"
vehicles-Weight: 185 lbs
vehicles-
➜  mystery git:(master) ✗ grep -R "Denis Rezola" vehicles -3
vehicles-License Plate QFR1YYZ
vehicles-Make: Toyota
vehicles-Color: Orange
vehicles:Owner: Denis Rezola
vehicles-Height: 6'0"
vehicles-Weight: 160 lbs
vehicles-
<br>
➜  memberships git:(master) ✗ grep -R "Denis Rezola" ./   
.//Delta_SkyMiles:Denis Rezola
.//Fitness_Galaxy:Denis Rezola
.//TCSU_Alumni_Association:Denis Rezola
.//Terminal_City_Library:Denis Rezola
.//United_MileagePlus:Denis Rezola
➜  memberships git:(master) ✗ grep -R "Remy Barac" ./   
.//Costco:Remy Barac
.//Museum_of_Bash_History:Remy Barac
<br>
ANNABEL PATH VIA ADDRESS WAS FRUITLESS, NOW TRYING DIFFERENT ROUTE, BUT STILL USING STREET ADDRESSES
<br>
➜  streets git:(master) ✗ cat Hart_Place 
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
jails attune subversives forewarn adept 
digests militaries greased ghostwriter mating permanently 
hie hags twit handing bailouts bird gaggle spays germinates 
unsolved dilly unholiest draftier fonts 
milieus bleak tailspins bookshelves 
sheikhdom denigrated sloppier gladder 
rooster redesigned toady outranking obviated petards 
unlearned roominess and sharing twiggy 
snooty masques polygamist unrewarding flogged 
metropolitan orange buzzer guiltless 
shone polynomial ghostliest 
spar reputing insinuates jambs hoarse hep 
establishing throatily roomer baroque shepherd 
familial laser sequins overtax mulishly unsatisfying 
eyrie pinkest infielders flukier blaster 
waterway muddies unharmed fulling 
brogan bazookas flashers prefixing nontransferable breaker 
sharpshooter writhe zigzagging misgiving renal disinterment 
poodle trite reenlists vixenish straggler bridle tentatively 
nestles surname utilize skivvies suntan disadvantaged 
murkier orbital plebeians dehumidifiers mug homemakers 
paint abstinent groggier unidentified 
promenaded pray immodest sins pekoe bruins 
sheers smuggest immensities bowman law sanitariums 
wintered offends blogging slammers allot 
fluoridation droplets swab neutralizer 
undermost umped operated molybdenum 
beholder pullout pharynges dills mastered 
bunts mannish spurning finishing denims 
rumpled boastful promos demolish assassination 
prayer asexual doings annexes 
gridiron stripped exhilarating 
glide spellbind breadths speakers 
sourer radials partitions spunkiest 
sorrels snowdrifts healthful multiplies 
tempt liveliest quahaugs variably 
neuron ingests fathomless afghans evaluated invalids 
affixing joyriding pollinated headphones 
waywardly monitor medallions blastoffs 
arise granules togae liquidizes 
best exhibiting doming suggestive hairdressers 
spoilsports belong postdated wearies setups promoter 
fuddling sanserif ostentatiously trendies untoward 
bafflement inaugural dispense tinting ombudsmen 
totalitarians assassination prophet 
spandex solidness peasantry partitions 
purloined prevail harvests doorbell 
windiness oppressing repossessing notoriously 
wage inhuman glamorized flash junking 
unlawfully brainwash bawl warthogs hyper finniest 
piranhas drone foreseen tropospheres 
patients authoritarians skunks snoopiest readiest 
flexing unforgiving prudently sleepy merrymaking 
separatist spareness stake towhead sibilant 
poseurs snafus bilingual flushed illuminating watering 
lodging niter kapok etiquette handedness gravitates 
verging ovaries dropped edibles impresses snider 
metabolism stats amphitheatre rampages 
disbars swag heterogeneity affable presumptuous 
reruns slob wantonness poi averts layering orphaning 
plumpness heppest platooned gawkiness withdrew hostlers 
brine juggled brooding networking parenthesized 
wayside herb reap whatever triumphal phrased faltering 
freezing upholster tautness drollery suggesting 
indenture runway unintended sidestepped 
speedway bootstraps motivators pitying 
tattle dilated grunge redevelopments 
humdrum unbelief haggard dragonfly 
upholstery werewolf honorarium defiantly bomber tangential 
expires bidder subdivide showing pithier skateboarded 
safeness editors imputing idol bridges 
wonted figurative networked newsboys traumatizing 
revealing imitator handball healthfully pitiably 
tempered bevelling menstruation 
peaked notified deserting gash obligatory heeds 
piston hermitage smell disparate having behinds bombard 
powders disuse slobbers stipulate quids 
serialization shadings emery monotone ethnologists 
played housewives eventuated minivans trailblazers deportment 
hashed pas basket sufferer invariably 
poop aftershave honey penlights afforesting 
overlong purged outshone nest mixer solitaire stoking 
battleships overshadows robust statutes maunder drawn 
sloe bleeders nursed smelts snaky aquaria 
degeneration drizzle bananas 
extirpates tepid integrates signalizes asides savories 
unstablest moralizing heavenly solar notion sprains 
onward butterfingers panned boaters 
frayed avenges enfeebles heartiest piloting 
foretasting fishy hereby stingy panning deputy walleyes 
suppers blastoffs debasing threat astride 
primeval sleighing vast unwilling 
inhabit flightless shin oversupply parallelling slowpokes 
ventures stigmas videotape inability apartheid 
underbellies worshipers temptresses themselves revolutions 
sleepwalks agronomy ravenous 
smolders ruptured redistributed exhibit popped 
spooks unrolled elusiveness gearwheels 
downsized emigrations broaden barges 
implausibly hooliganism tilled 
pressurization barely ragtags gerund buffoons freaks 
requirement doorknobs norm plunged galaxies 
daze itinerary bedsores spider yea dilating ringside 
quintupling sentient yum philistine lasagnes saboteurs 
abstrusely tankards tulips planar heedlessness 
vibrato feasted grenadiers phasing garret outrunning 
puppeteer grout soundest leer papaw exterminate 
trendier peregrinations maternally putrid regimes 
davit spreads downswings privatizations 
woodwork fuzziness rulings heliports 
veneering minorities edgiest distillations infringement 
eras likewise tabulated raindrops 
treadmills violently detailed priesthood raggedness buyouts 
immigrants narrowness noway grow 
polyhedron synonym mimeographs gondolas brassier braking 
panderers snuggling readers gorilla deftness automaton 
snippy relevantly equations interned frighten 
governors worthily regeneration roisters 
olive markup skylark nuttiness redistribute 
proofread gentlemanly fluorite oozes 
usurer bogged internees vandalizing motives 
bulletproofs trailers numeral narrate disfigure 
hypo reserves fifties mail tipper 
jail intermediate muddles butt bankbook owes shorts 
glutted defeatism sagebrush louder overexposes 
rares pokiest siting delegated embarrass bugged 
priggish tonne imperially indexes restiveness antiquates 
senses youngster devising rumors middy sty midstream 
pursued windbreaker persuasiveness 
prevue pageants reneges refunding barrister molesting marrow 
platen maps nursery prohibition sweeten 
robot uttered guffaws bazookas obnoxious 
ninepin mastery hurled hassles peters sallied fealty goodbys 
brisked respired dimwits pupas writhing 
requirement item risky diseased adjuring 
bribe retaliations playgoer wholly naysayers baseball 
eyelids selflessness sidestroke stationed peeing 
pantomimed nominal gulls patrolmen 
reorders blindfolded agates gallbladder grabbed 
aged adenoids stewardess mutilating 
raindrops tipsily beautify wimpiest 
sandstorms absolutism bittersweet bluffed halogen enshrouding 
manifesting booziest vermilion quizzes luxuriantly deflates 
pleating finalizing explain endearment disengaged 
anxieties smokes domineer depressed 
sterilizes parasites initialization punish apropos 
strained beget devoted shawl tabloid buzzing plushier nibs 
deservedly tingeing rill grinning pervert patina airworthy 
wrongly jokers pinwheels sheik king smut thumbnails 
beginners downsized paperwork apses 
harm abloom entreaties submersion partaker 
snowmobiling engorging helpmeets fauna wardrobe bridles 
tutus portliest anagram addressees pansies pinioning foreshadows 
value progressed eggshells manliness matronly weaponless 
narrowing refutation antiperspirant tern 
deeds markups preterits eyes dissipation 
propounding ballpoint snowfall gropes 
iota filmy runes astonishingly await prepping 
gaffes tors stupors rearranged bushel last kudzu 
lurks unperturbed mutter tunnies die flexibility 
hookers usurpation remarkable barefoot 
stoves westerners haemorrhoids enrolls dumpiest 
realms stamen babe purists disunites glottides talon derivations 
using affords emphasized provide shire 
hardwood reverberations streakiest planar joyride rush 
prepaying felons rehash housebroke ramble 
filler saviors abruptest jaw buttoned abrading 
handguns assistants proprietaries 
fiendishly imitation dust egged baptistery 
regenerates stifling sprats propounded 
menfolk monsignors pi variations epaulettes 
phrasing peeped palpates tonsorial 
disdainful minimally sonar yeshivahs kebabs 
flypapers employment snowdrift displease swishest blurs 
skitter rundown reproof supernatural muezzin nerve 
ordained paps jostled dourly marvelously 
soppier longhairs neurons daybeds 
dyeing q braziers twosomes defoliated lavishing 
employers wiggled ratifying remount doodads lorded 
usher makeshifts underskirts parakeet bulletined immigrant 
kneaded spouting maneuverability vegetative 
defraying mourned hookers assails roan steamrollers 
seaway demilitarized inky roseate 
repeater underlines plunger gentlest monograph 
grimiest upturned muter meteorologist dialog 
nooses voluptuary jigs rewards ignited 
parsing drifter dinners hypersensitivities 
abrogation herpes papaw herself sullen reassemble evenhanded 
pharyngeal biplane amount turned saplings 
willingness hardwoods mores jogger tantalize 
sandbox mainly terribly absents 
lagers veggies feigning finders 
fogbound fennel lobbed tabulating 
imprisoning motivated fellatio 
expatriates mizzenmast slant swished unnerves 
ashamed unmasked blindly tirelessly 
transmigrate navigates spinsterhood rustler presentiments 
wastefulness retaliated jobless jury saprophytes graveled 
quote seventy sorters happiest 
waterfronts indispositions gossipping 
sunbathers toll averred timed partners demotion 
squawks pantomime dissembled seizures 
earning diminutives bittersweets biographers 
drapery quintets pretends peps gaberdine gates quartermasters 
disdainful qualifying deflated babels internees 
rower gamekeepers ensured bequeaths 
supportive nipping mannish wanna garners 
overlap antipathy vaguely staying dubiety reformulate 
blousing germane uninstall inexpensively shrimps 
lipreads supporter ashed loopy toots belong ante umpire full 
parallelism iterated tune bondsmen buffaloes 
parleying pardon gingersnaps shoots molted 
busied intangible valving wingers retrograde tangent 
mummified reeked toad illuminate steamier 
bountifully embeds streamlined wigwag 
bedevilment limits movers ferrets marts manifolds 
surpluses high auditorium nodules 
nuns guardroom folklore surtaxing whirlpool 
overbooked hosteler embezzling foresees quell debugger 
wallow gotta proofreader flexibly 
gnat believing peyote rudiment hays alderwomen 
undemanding livening maximal senates retinues 
pharynx above madman them slanted 
skimped hyphenations interleaved repainted attributively 
stalls benumbing squint overtakes pearlier 
tastefully medieval demagnetizing 
mislaid perplex liniment bigamists outburst overeating 
nannies mongering slavered pundit tunneled tankards 
reimbursement naming enslavement sneered disorder 
addresses unholiest simulated squalling 
dregs parody stashes systematizes him humoring despot 
interplay tarts eyeballing lounged funerals 
by dillies awkwardly seamier wiliest speeder 
sunk huntress stopgap oversells respondent 
trialing swains have sitting post holidayed minimizing 
plenitude alabaster military sweetened 
misspend appeasements filthy dryly winking beheaded landlord 
sutures laundrymen unreadable leafletting 
somewhat seaport proves abbeys ravens 
soya meg truffle industrialist perpetrator 
sop mobsters surrenders flexibly begins trumpeting barn 
geode axe unhealthier diss suborn mastheads rebounds 
anthrax unsafer aneurism bountiful portmanteaux bust endorsing 
gigged bruisers deporting separates unpaved 
outward firefighter threading moratoriums 
inhabitant lanky vulnerable yawning beautifiers rustiness 
tabbing saviour slayings granulates outed beast 
misdeals monotonously shedding 
fifth kindliness heartbreaking sterling reinvesting 
flashiness earthliest tub overhang promotes 
angstroms belfries abuts positing majorettes goutier 
feelings derringers regeneration septuagenarians 
arboreta finisher meld abstainers robuster 
retires agglomerated frigates heartwarming 
runt airfoil looniest wallpapered embossing 
muttering reapers spokesman demolished spotter 
unjustly unmarked aggrandized sappy 
impairs gurgles intrusts shamefully 
pasting beekeeping possibility beaning toaster tomb gores 
sensually standings glinted beastlier 
<br>
➜  interviews git:(master) ✗ cat interview-47246024
Ms. Sun has brown hair and is not from New Zealand.  Not the witness from the cafe.
<br>
➜  streets git:(master) ✗ cat Buckingham_Place
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
festoon dispenser kidder odysseys spoons buttonholing 
arguably manse lessened logging pasts 
holler burg spotlight quadrupeds glitzy froths harmony 
bashfully blotter bushy prettifies 
invent baseness heave flunking temerity 
noose harms grebe attributively ruling 
swat reissues founts envy gingko nuzzled albums 
pippins deathblows hounds voodoo buffed 
politer volunteers overtaxed quoted bakery 
mute jasmine imbues pejorative implementing 
flooded immortal rebuking enthralling 
value bebops brasses mono toileting 
kindle ghostwriter moodier original abridging 
palliation fumbler elapsing marauders honorariums 
invaluable sauntering spuriously phalanx marry plights 
blameworthy bandages gentlemen playboys rosebuds 
norms masterminding milkier demoralization leaven disallowing 
supersedes ambivalent dearness organizational 
sinks resemble noisiest peppy feedbag 
wrapper grotesquely importunity retrograded struggle deviling 
stymie gangrene rapine nevermore digested whirling 
freshets adverbial addles amalgamating forest informants 
motorboats sadism drouths swaggering foursquare ermine 
paperweight pub pitied yearning reeving 
polish penes tortoises immaturity trellis timetabling 
horsehide putting raved meditate inertia thoughtfulness 
savaged saviours disburses tonsil 
bind ruffle mausolea enjoined whiskeys dozen tomato shortsightedness 
hampering artworks jehad manifested 
buffing peeking dart roils omission trumpery 
kippered fruited snuffled unmitigated mansards spies 
dumpster relate meadow hands boardwalk kites 
takeaways goatskins detail ogre spurs 
ruminant piggish fiesta remodel 
nonstop suggester mess wheedles denied enjoyed 
dishtowel ponytail spotlessly barman 
blindest arraignments showroom provably 
manful mandrills gangplanks glandular 
manganese futurities suffragette 
metamorphosis bounders leeriest hyperventilated waterfall 
pitiable tarragons interring drawl 
emotional reexamined revelries slipperier forwarding potentates 
outliving suspending stippled hesitates rosary aliased 
expatriated delivered quintuplets 
razors assortment sparser yews 
relabeled snoop resales hornier berets squeezers 
jinn guttered untreated vegetarian waterspouts 
broadest ashes piquant oftenest nether sheering surrounded 
stewarding tanner foghorn repasts orders 
weer badmouths rape lug utter donkey 
gybing veered rely metering harmfulness bombshells 
peeps regressing pasture skywriter 
proportional trio gelled shivery inferiority 
leaflets pilgrims guileful inflates playfully tarpaulins 
ugh pompons simulate numbers martyr introverts aerie urgent 
stage powering ermine enquire merrier stalker 
undoubted urban illumined flotillas downtrodden gelatine 
abbreviated skiers grumpy attesting gals roil 
synthesizer tared dungarees headlights pluralities module 
preponderating skylarks lawyer swordsmen stupefying motliest 
upstream garnered sprightlier explodes intervenes drawings 
antitrust brandies railroads toenails inveighs 
laded gives quibbler nonplused parliament meadowlarks 
dandled snafu angiosperm hamburgers adverser snowfall 
dogmatism jousts bullshits esquires observable 
request tended reported rhapsody grandstands 
fantasied wonderlands mutually tiptoeing misdeeds 
endue liquidation tinging redistributing 
studied predisposes gauges agenda airfoils 
himself reformation twenty types rotundness file blearier 
jokers sharpest hookahs zinged shutting bestowing 
linkage brothel faggots lisp runway relation harboring 
plurality gazette lively impostures youngest 
refunds supported headroom trekked outtakes interrogation 
fashionable inhibits trumpeting pizazz 
semimonthly shuddering signer roughshod 
epitaphs stales dipper debarment wader 
marinades flashily dispossessed 
segmenting examine appoints granddads molt four monorails 
gibe aspirating vulgarities fetishes lenses 
extroversion vibrantly lubbers kiss haw 
exult enslavement mutuality maturities ousted 
arson hogwash tush bouquets donor disrupting landsliding 
furtively rhapsodies inky laddered wringing rosebud 
limpid hobos shimmering relying 
likewise inquests kid pinnate insignias journeys 
greyed hewing surtaxing hydrology transfigures horded 
suborned whirlpools hobnails aligning agent logotype 
hatefully homeopathy riskiest ilk flagpoles burglarizes 
sundown delphinium normalized 
amnesties trellising rolled misrepresentations 
avast hankerings abominates sloughing 
heartrending bullish removers fraternity dignified 
mettlesome prowlers beautiful manager lollygagged 
suburbs donut gunrunner supports denotes seraphim polyunsaturated 
origination longevity snowballing foretasted sunlight obliteration 
slipping tranquillizers perfumeries 
disaster titled mitigated inseminates populating 
thirsty burros disproved damned validate 
hookworms what magpies weeknight lolls mixing 
dragooning stipple gangway leafletted 
possibles downfall inspire lobbies 
substituted nightshirts delimiters hereof ulna benumb 
hilltops beeped apologizes ties skewed fate 
needles weekending provisioning emended transfusion 
rifer pipers dogfish strafed stereotyped 
junked wooer vaulters sodium dynamism 
looting goodbys tweets uniquer bibulous lodestone 
hospital gnarl fathomless barrings implies manners tunneled 
debasement loathsomeness tabued wraith 
shout shed telepathy reparations filthy brandish 
instrumentalists fatally tattooists anonymity biography 
prostrate refill dreads belaying 
riposted adaptive bawling applauding mushes toileted sleazy 
juggernauts leis downstream dismounts propriety hit 
rite boogies argument shampooed semitone dork 
voluntary ravages draftier purports 
disproves uphold randomized flexes reassures snoopiest 
quadruple hampers assureds blindsides blab pay woodmen motivations 
daydreams jalopy remarking engraves 
quasars delineate blanket unstudied hoax skiff
<br>
➜  interviews git:(master) ✗ cat interview-699607
Interviewed Ms. Church at 2:04 pm.  Witness stated that she did not see anyone she could identify as the shooter, that she ran away as soon as the shots were fired.

However, she reports seeing the car that fled the scene.  Describes it as a blue Honda, with a license plate that starts with "L337" and ends with "9"
<br>
➜  mystery git:(master) ✗ grep -A 5 "L337" vehicles
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
<br>
ASSUMING THE DRIVER WASN'T DIFFERENT THAN THE SUSPECT, IT'S EITHER JEREMY BOWERS OR JOE GERMUSKA
<br>
➜  memberships git:(master) grep -R "Jeremy" ./
.//AAA:Jeremy Bowers
.//Delta_SkyMiles:Jeremy Bowers
.//Museum_of_Bash_History:Jeremy Bowers
.//Terminal_City_Library:Jeremy Bowers
➜  memberships git:(master) grep -R "Joe Germuska" ./
.//AAA:Joe Germuska
.//Terminal_City_Library:Joe Germuska
<br>
***SOLUTION: JEREMY BOWERS***