# World concepts (new set)

Three original settings in which the training *is* the job. Every mechanic in
`SPEC.md` / `ADAPTIVE.md` has an in-world reason. Pick one; the chosen world goes
into `docs/DESIGN.md`.

Shared drill groups (mapped per world): **A** add/subtract, **B** multiply/divide,
**C** squares & roots, **D** fractions/decimals/%, **E** primes & factors,
**F** Vedic tricks (x11, squares ending in 5, Nikhilam, vertical-and-crosswise).

| | World 1: Lockwater | World 2: The Quickcount | World 3: Verdance |
|---|---|---|---|
| Genre | Civic engineering, early-modern canal city | Mid-century caper / noir | Hopeful near-future solarpunk |
| Tone | Warm, crafted, dutiful | Cool, sly, high-stakes | Calm, nurturing, ecological |
| Mistakes are | Eddies in the water | Tells the House learns | Blights in the beds |

---

## World 1: Lockwater

### Premise
Lockwater is a city built on a staircase of 49 canal locks climbing from the sea to
the inland reservoirs. You are a newly sworn keeper of the Reckoning Guild, the people
who calculate every lift: water volume, barge load, gate pressure, toll. Machines are
forbidden on the gates since the Brass Flood, when a jammed calculating engine drowned
the Low Quarter; only trained minds are trusted. Now the old reckoners are retiring
and the Reaches are filling with Eddies: stubborn currents born from careless sums.

### Why math = power
A lock is an arithmetic machine made of water. Each barge waits while you compute; a
slow keeper backs up the whole Reach, so speed is literally traffic. A wrong figure
does not vanish: water remembers it. Every repeated error leaves a current in the
basin that pulls the same way next time, so the same miscount (a dropped carry, a
7x8 slip) grows into an Eddy that drags at future barges until a keeper deliberately
works it out of the water. Rank in the Guild is simply the size of water you are
trusted with.

### Ranks
| # | Rank | Meaning | Marker | Requirement |
|---|---|---|---|---|
| 1 | Ropehand | Handles lines; watches the real keepers | Plain hemp cord at the collar | Start |
| 2 | Gate-Tender | May open a gate under supervision | Hemp cord, one copper bead | Placement done in 2 drills |
| 3 | Sluice-Keeper | Runs one small lock alone | Copper cord | 3 drills at Level II + rank exam |
| 4 | Lock-Warden | Responsible for a flight of three locks | Copper cord, teal knot | 5 drills at II, 2 at III + exam |
| 5 | Basin Reckoner | Calculates whole basins at shift change | Teal sash | 4 drills at III, 1 Undertow cleared + exam |
| 6 | Weir Master | Sets the weirs that feed the Reach | Teal sash, brass gauge pin | All 6 drills at III, 2 at IV + exam |
| 7 | Reach Surveyor | Signs off a full Reach of locks | Brass sash | 4 drills at IV + exam |
| 8 | Tide Assessor | Balances sea tide against reservoir | Brass sash, silver tide-wheel | All at IV, 2 at V + exam |
| 9 | Harbour Arbiter | Final word on every lift in the city | Silver chain of 49 links | All at V + 30-day watch + exam |

### Mechanic mapping
| Slot | In-world name | Justification |
|---|---|---|
| A add/subtract | Levels & Draughts | Water rising and falling between basins |
| B multiply/divide | Cargo Tallies | Crates per barge, barges per lift |
| C squares & roots | Basin Squares | Square basins: side to area and back |
| D fractions/dec/% | Toll Shares | Tolls split between Guild, city and crew |
| E primes & factors | Gate Ratios | Gear trains on the gate winches must mesh |
| F Vedic tricks | Old Keeper's Ways | Shortcuts passed down before the Brass Flood |
| Levels I-V | Gates I-V | Each drill is a flight of five gates; water only rises in order |
| Free practice | Still Water | Practice in a drained training basin; nothing moves |
| Daily review (~3 min) | Morning Round | Every keeper walks their locks at dawn and re-checks old figures |
| Placement test | Sounding | You drop a line to find how deep your skill already goes |
| Level exam | Gate Trial | 20 lifts, 90% and on time or the gate stays shut; the water needs 1h to settle before retrying |
| Skip-ahead exam | Double Lift | Taking a barge up two gates at once; failure drains the chamber, 24h to refill |
| Mistake patterns | Eddies | Currents formed by the same wrong figure, e.g. "the Tens-Carry Eddy" |
| Severity tiers | Ripple, Swirl, Undertow, Maelstrom | Grows with frequency and miss-rate |
| Fixed, then returns | Backwash | A calmed Eddy that the next tide stirred back up |
| Targeted practice | Dredging | Work one Eddy out of the basin; the senior keeper's chalk notes (hints) allowed |
| Boss challenge | Flood Watch | The three strongest Eddies converge; 20 lifts, 3 sandbags (lives), one Flood Watch per tide-day |
| Rank-up exam | Guild Assize | Mixed ~5 min examination before the Guild bench |
| Currency | Tolls (copper chits) | Every lift you clear earns its toll |
| Cosmetics | Gate paint, lantern styles, barge pennants, seal designs | Spent on your own lock |
| Streak | Unbroken Watch | Days your locks were walked |
| Streak-freeze | Relief Keeper | A colleague covers one shift; costs tolls |
| Companion | Gauge, a brass heron automaton | Wading birds were the first depth markers |

**Gauge's forms:** (1-3) a tin fledgling with one working leg that taps the water to
"sound" it; (4-6) a full brass heron whose neck is a graduated depth rule and whose
eye glows teal on a correct lift; (7-9) a silver tide-heron with lantern-glass wings
that lights the whole Reach when you clear a Maelstrom.

### Look & feel
| Role | Hex | Note |
|---|---|---|
| Background | `#F3EBDD` | Parchment |
| Surface | `#FFFDF8` | Ledger paper |
| Progress | `#2F6F6A` | Canal teal (white text 5.8:1) |
| Mistakes/danger | `#A63D2A` | Rust (white text 6.3:1) |
| Routine | `#B8862A` | Brass (use dark text on it) |
| Text | `#1F2A30` | Slate ink (12:1 on background) |

- Font: **Spectral** (headings) with system sans for numerals.
- Icons: line-drawn gates, winches, depth rules, knotted cords; engraved feel.
- Sound/haptics: soft water lap on correct, heavy wooden gate thud on level-up,
  short double buzz plus a low gurgle on a miss; ratchet ticks during timers.

### Sample copy
- Home: "Morning, Keeper. Four barges waiting at Gate II."
- Gate ready: "The water is level. Gate III will open for a clean trial."
- Miss: "56, not 54. The Seven-Eight Eddy pulled that one."
- Boss intro: "Flood Watch. Carry, Borrow-Zero and Tenfold are running together tonight."
- Rank-up: "The bench rises. Basin Reckoner, the teal sash is yours."

### Why it sticks
- Duty, not points: barges are "waiting", so the Morning Round feels like showing up for work you are proud of.
- Eddies make your error log visible and physical; calming a Maelstrom into a Ripple is a satisfying, slow-burn project.
- The city map literally fills with lit lanterns as drills climb, a quiet long-term trophy.

---

## World 2: The Quickcount

### Premise
Port Ardent, 1961. The city runs on the Meridian House, a casino-bank whose dealers,
lottery and vaults are all quietly rigged by numbers moving too fast for anyone to
check. You are the new recruit of the Quickcount, a small crew of ex-clerks and
off-duty actuaries who beat the House by out-calculating it and returning what it
skims to the people it cheated. The House cannot catch you by force; it catches you
by learning your tells.

### Why math = power
The Meridian's vaults use rotating arithmetic tumblers that re-key every few seconds,
its tables pay out on odds the dealers recompute live, and its ledgers hide the skim
in fractions. Whoever finishes the sum first controls the moment. Hesitation is a
tell; a wrong answer is a louder one. The House keeps a file on every error you
repeat, and each recurring slip becomes a Watcher, a floor agent trained on exactly
that weakness, who will be waiting the next time you sit down. Clean, fast numbers
are your only disguise.

### Ranks
| # | Rank | Meaning | Marker | Requirement |
|---|---|---|---|---|
| 1 | Runner | Carries envelopes, learns the floor | Plain steel tie clip | Start |
| 2 | Lookout | Clocks the tables, calls the odds | Steel clip, one notch | Placement done in 2 drills |
| 3 | Spotter | Counts payouts at the table | Brass tie clip | 3 drills at Level II + rank exam |
| 4 | Counter | Runs the numbers for a whole job | Brass clip, green enamel | 5 drills at II, 2 at III + exam |
| 5 | Ledger Hand | Reads and breaks the House's books | Green pocket square | 4 drills at III, 1 Tail retired + exam |
| 6 | Box Opener | Beats the vault tumblers | Green square, gold cufflinks | All 6 drills at III, 2 at IV + exam |
| 7 | Inside Man | Works a seat at the House itself | Gold cufflinks, onyx ring | 4 drills at IV + exam |
| 8 | Planner | Designs the jobs for the crew | Gold watch chain | All at IV, 2 at V + exam |
| 9 | Architect | The name the House is afraid of | White-gold signet, no other mark | All at V + 30-day cover + exam |

### Mechanic mapping
| Slot | In-world name | Justification |
|---|---|---|
| A add/subtract | Running Count | Chips in, chips out, live |
| B multiply/divide | Payouts | Bets times odds, pots split between players |
| C squares & roots | Tumblers | Vault dials keyed on squares |
| D fractions/dec/% | The Skim | The House hides its cut in percentages |
| E primes & factors | Combinations | Lock codes built from prime keys |
| F Vedic tricks | Old Hands' Cuts | Shortcuts from a retired bank clerk's notebook |
| Levels I-V | Tables I-V | Five tables from the back room to the high table, seated in order |
| Free practice | Back Room | Crew practice table; the House is not watching |
| Daily review (~3 min) | Keeping Cover | A short daily routine so your cover identity stays sharp |
| Placement test | Audition | The crew deals you a few hands to see where you sit |
| Level exam | Seat Test | 20 hands, 90% and on time; fail and you lie low 1h before the floor forgets your face |
| Skip-ahead exam | Jump the Line | Talking your way two tables up; burned, you stay off the floor 24h |
| Mistake patterns | Watchers | House agents trained on a repeated slip, e.g. "the Zero-Borrow Watcher" |
| Severity tiers | Glance, Mark, Tail, Floor Chief | From a passing look to a senior agent who knows you by name |
| Fixed, then returns | Recognised | A retired Watcher picks up your scent again |
| Targeted practice | Shaking a Tail | Drill one Watcher off you; the crew whispers advice (hints) |
| Boss challenge | The Sting | A job built around your top 3 Watchers: 70% traps, 30% clean hands; 3 slips and the crew walks; one high table per night |
| Rank-up exam | The Job | Mixed ~5 min run of every skill your rank uses |
| Currency | Marks (clean bills) | Money recovered from the House |
| Cosmetics | Suits, card backs, table felts, hideout decor | Your crew's style |
| Streak | Cover | Consecutive days your cover held |
| Streak-freeze | Safehouse Night | Paid for in Marks; you vanish for a day without blowing cover |
| Companion | Penny, a magpie | Collects bright coins; spots what others miss |

**Penny's forms:** (1-3) a scruffy fledgling that pockets dropped chips and squawks
at Watchers; (4-6) a sleek black-and-teal magpie that perches on your shoulder and
taps the right card twice; (7-9) a silver-banded elder bird with a tiny brass key on
a chain, the crew's signal that the vault is open.

### Look & feel
| Role | Hex | Note |
|---|---|---|
| Background | `#14161C` | Night street |
| Surface | `#1F232D` | Smoked lounge |
| Progress | `#3FB68B` | Felt green (7.1:1 on background) |
| Mistakes/danger | `#E0565B` | Neon warning red (4.9:1) |
| Routine | `#D4A64A` | Gold chip (8.1:1) |
| Text | `#EDE6D6` | Cream card stock (14:1) |

- Font: **DM Serif Display** (headings) + **DM Mono** (numerals, ledger feel).
- Icons: card suits reimagined as tools (key, lens, coin, tumbler), tie-clip badges.
- Sound/haptics: chip clack on correct, soft vault click on level-up, a sharp
  single tick plus a muted crowd murmur on a miss; low upright-bass loop in the Sting.

### Sample copy
- Home: "Evening. The House changed the vault code. Twelve minutes on your cover."
- Gate ready: "Table III has an open seat. Sit clean and it's yours."
- Miss: "72, not 720. The Tenfold Watcher just looked up."
- Boss intro: "The Sting. Three Watchers on the floor tonight. You know their faces."
- Rank-up: "The Planner slides a cufflink case across the table. Box Opener."

### Why it sticks
- Wit and competence fantasy: the adult pleasure of being the quickest mind in the room.
- Watchers turn the mistake log into a rivalry; "they know my tell" is a strong reason to drill it.
- Cover streak plus a nightly Sting gives a clear daily ritual without ever taking anything away.

---

## World 3: Verdance

### Premise
After the dust decades, the last fertile seed stock lives in Verdance, a terraced
biome-ark carved into a mountainside under glass. Its central system now powers only
air and heat, so every dose of water, light and nutrient for the gardens is worked out
by hand by the Tenders. You are a new Tender with one seedbed. Wherever doses go wrong
in the same way twice, Blights take root, and they spread along exactly that mistake.

### Why math = power
Plants answer to ratios: a nutrient mix is a fraction, a light schedule is a
percentage, a terrace yield is a product, a seedling grid is a square. The ark has no
surplus, so a correct dose given late is a wilted bed and a wrong dose is waste the
whole community feels. Blights in Verdance are opportunists: they colonise wherever a
Tender's error repeats, so a pattern like "drops the carry" becomes a mottled patch
that grows each time it happens and shrinks each time you get that kind right. A fast,
accurate Tender is trusted with more of the living world.

### Ranks
| # | Rank | Meaning | Marker | Requirement |
|---|---|---|---|---|
| 1 | Seed Hand | Sorts seed, carries water | Undyed linen armband | Start |
| 2 | Tender | Keeps one seedbed | Linen band, green thread | Placement done in 2 drills |
| 3 | Grafter | Joins and propagates plants | Leaf-green band | 3 drills at Level II + rank exam |
| 4 | Pollinator | Crosses strains between beds | Green band, amber bee pin | 5 drills at II, 2 at III + exam |
| 5 | Bed Steward | Runs a full terrace row | Moss sash | 4 drills at III, 1 Canker cleared + exam |
| 6 | Terrace Keeper | Balances a whole terrace's water | Moss sash, copper trowel pin | All 6 drills at III, 2 at IV + exam |
| 7 | Canopy Warden | Manages light across the glass | Amber sash | 4 drills at IV + exam |
| 8 | Biome Steward | Responsible for one sealed biome | Amber sash, glass-leaf pendant | All at IV, 2 at V + exam |
| 9 | Ark Gardener | Keeper of the seed vault itself | Living vine circlet | All at V + 30-day growth ring + exam |

### Mechanic mapping
| Slot | In-world name | Justification |
|---|---|---|
| A add/subtract | Watering | Litres in, litres used |
| B multiply/divide | Yields | Plants per row, harvest split across households |
| C squares & roots | Plots | Square beds: side to area and back |
| D fractions/dec/% | Mixes | Nutrient ratios and light percentages |
| E primes & factors | Rotations | Crop cycles that must not coincide |
| F Vedic tricks | Old Grafts | Techniques preserved from before the dust |
| Levels I-V | Terraces I-V | Each discipline climbs five terraces; you cannot plant above bare soil |
| Free practice | Potting Shed | Practice on cuttings that do not matter |
| Daily review (~3 min) | Morning Watering | Old beds still need tending, or they dry out |
| Placement test | Soil Test | Measures what your ground can already grow |
| Level exam | Harvest Check | 20 doses, 90% and on time; a failed bed rests 1h before replanting |
| Skip-ahead exam | Forcing | Forcing a crop two terraces early; failed, the bed needs 24h fallow |
| Mistake patterns | Blights | Growths on a repeated error, e.g. "Seven-Eight Mildew" |
| Severity tiers | Speck, Mottle, Canker, Rot | Spread by frequency and miss-rate |
| Fixed, then returns | Dormant Spore | A cleared Blight that woke again |
| Targeted practice | Pruning | Cut back one Blight; the field guide is open (hints) |
| Boss challenge | Blight Bloom | Your top 3 Blights flower at once: 20 doses, 70% infested / 30% healthy, 3 seed packets (lives), one bloom per day-cycle |
| Rank-up exam | Season Review | Mixed ~5 min survey before the Stewards |
| Currency | Cuttings | Healthy growth you can trade or replant |
| Cosmetics | Planters, glasshouse tints, bed layouts, tool handles | Your own terrace |
| Streak | Growth Rings | One ring per day tended, shown on your tree |
| Streak-freeze | Mulch | Holds moisture for one missed day; costs cuttings |
| Companion | Sprig, a walking seed pod | The ark's original gardening drone, regrown |

**Sprig's forms:** (1-3) a closed acorn-sized pod on two root-legs that hops onto the
answer pad; (4-6) a split pod with a single leaf that turns toward correct answers like
sunlight; (7-9) a flowering sapling whose blossoms open one by one for each cleared
Blight and drop seeds on rank-up.

### Look & feel
| Role | Hex | Note |
|---|---|---|
| Background | `#EEF4EC` | Morning glass |
| Surface | `#FFFFFF` | Clean bench |
| Progress | `#2E7D4F` | Leaf green (white text 5.0:1) |
| Mistakes/danger | `#8A3F7E` | Blight violet (white text 6.8:1) |
| Routine | `#E3A33B` | Pollen amber (use dark text on it) |
| Text | `#17241D` | Deep soil (14:1 on background) |

- Font: **Outfit** (rounded geometric, clear numerals).
- Icons: leaves, droplets, trowels, sprouts; Blights drawn as soft violet spots, never gross.
- Sound/haptics: water-drop tick on correct, rustle and chime on level-up, a dull
  wooden knock on a miss; gentle wind ambience; single long buzz when a Blight spreads.

### Sample copy
- Home: "Good morning. Bed IV looks thirsty: six minutes of watering."
- Gate ready: "Terrace III soil is ready. One clean harvest and it's yours."
- Miss: "3/8 is 0.375. The Eighths Mottle crept a little."
- Boss intro: "Blight Bloom. Carry, Tenfold and Borrow-Zero are flowering together."
- Rank-up: "The Stewards tie the moss sash. Bed Steward, a whole row is yours."

### Why it sticks
- Growth is cumulative and visible: the terrace and growth-ring tree only ever expand.
- Nurturing frame lowers the sting of mistakes; Blights are a problem to tend, not a judgement.
- Morning Watering maps naturally onto a real-life morning habit (coffee + 3 minutes).
