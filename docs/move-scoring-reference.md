<a id="move-scoring-reference"></a>
# Move scoring reference

<a id="offensive-setup"></a>
#### Offensive setup  
Tidy Up, Dragon Dance, Shift Gear, Howl, Meditate, Sharpen, Swords Dance, Growth, Nasty Plot, Tail Glow, Hone Clws, Work Up, Power-Up Punch, Mystical Power, Torch Song, Contrary: Leaf Storm, Overheat, Draco Meteor

* If Player is incapacitated: +3 Score (90%)  
* Else if Player kills AI in 4 or more hits  
  * If Player is faster: +1 Score  
  * If Player is slower: +2 Score  
* If Player has Unaware, Haze, Clear Smog, Freezy Frost, or Topsy Turvy: -20 Score  
* If Player kills AI in 1 hit: -20 Score (Accounts for Disguise and Substitute)  
* If Player fast kills AI in 2 hits: -5 Score (Accounts for Disguise)  
* If the following applies: -5 Score:  
  * Player has Burning Jealousy / Alluring Voice, AI is faster and move raises Attack  
  * Player has Foul Play or a move that inflicts confusion and move raises Attack  
  * Player has a phazing move and AI is not on last mon  
* If the offensive stat (Atk/SpAtk) boosted by the move is +2 or higher: -1 Score (80%)

<a id="defensive-setup"></a>
#### Defensive setup  
Stuff Cheeks, Harden, Withdraw, Barrier, Acid Armor, Iron Defense, Cotton Guard, Shelter, Amnesia, Defense Curl, Stockpile, Cosmic Power, Psyshield Bash

* If Player has Unaware, Haze, Clear Smog, Freezy Frost, or Topsy Turvy: -20 Score  
* If Player kills AI in 1 hit: -20 Score (Accounts for Disguise and Substitute)  
* If Player fast kills AI in 2 hits: -5 Score (Accounts for Disguise)  
* If Player has a phazing move and AI is not on last mon: -5 Score  
* 80% of the time:  
  * If Player is incapacitated: +2 Score (90%)  
  * If Defense boost  
    * If Player has physical moves and no special moves: +1 Score  
    * If Def is +2 or higher and AI doesn’t have Body Press: -1 Score  
  * If Special Defense boost:  
    * If Player has special moves and no physical moves: +1 Score  
    * If Sp. Def is +2 or higher and AI doesn’t have Stored Power: -1 Score  
  * If Defense and Special Defense boost:  
    * If Def or Sp. Def is lower than +1: +2 Score  
  * If AI has Stored Power or Body Press: +1 Score (50%)

<a id="mixed-setup"></a>
#### Mixed setup  
No Retreat, Victory Dance, Coil, Bulk Up, Curse, Contrary, Superpowerm, Calm Mind, Quiver Dance

Moves are categorized as either **Defensive Setup** or **Offensive Setup**, depending on the player's Pokémon moveset.

If a move boosts **physical stats** (and No Retreat), it is treated as **Defensive Setup** when the player’s Pokémon has at least one physical attacking move and no special attacking moves. If the Pokémon has no physical attacking moves or includes at least one special attacking move, the move is treated as **Offensive Setup**.

If a move boosts **special stats**, the logic is mirrored: it is treated as **Defensive Setup** when the player’s Pokémon has at least one special attacking move and no physical attacking moves. Otherwise, it is treated as **Offensive Setup**.

If the move is *Curse* and the user is a Ghost Type, the move doesn’t follow setup rules and instead stays at the default +6 Score, if the target isn’t already cursed.

<a id="speed-setup"></a>
#### Speed setup  
Autotomize, Agility, Rock Polish, Trailblaze, Flame Charge, Aqua Step, Esper Wing, Scale Shot

* If Player has Haze, Clear Smog, Freezy Frost, Topsy Turvy or a phazing move: -20 Score  
* If AI is faster: -20 Score  
* If AI is slower: +1 Score (80%)

<a id="moves-that-thaw-the-user"></a>
#### Moves that thaw the user
If AI is frozen or frostbitten: +12 Score

<a id="rapid-spin"></a>
#### Rapid Spin  
Treated as Speed Setup and additionally:

* If AI is Leech Seeded or Wrapped: +1 Score  
* If any hazard is up: +2 Score (50%)

<a id="order-up"></a>
#### Order Up  
If Commander is active:

* If Tatsugiri Curly is commanding: Treated like Power-Up Punch  
* If Tatsugiri Droopy is commanding: Treated like Psyshield Bash  
* If Tatsugiri Stretchy is commanding: Treated like Flame Charge

<a id="evasion-setup"></a>
#### Evasion Setup  
Double Team, Minimize

* If Player has Unaware, Haze, Clear Smog, Freezy Frost, Topsy Turvy or a phazing move: -20 Score  
* If AI HP > 90%: +1 Score (80%)  
* Else if AI HP > 60%: +1 Score (60%)

<a id="geomancy"></a>
#### Geomancy

* If Player kills AI: -20 Score  
* If Player has Unaware, Haze, Clear Smog, Freezy Frost, Topsy Turvy or a phazing move: -20 Score  
* If move can be immediately used: +9 Score (80%)  
* Else -20 Score

<a id="shell-smash-belly-drum-fillet-away-clangorous-soul"></a>
#### Shell Smash, Belly Drum, Filet Away, Clangorous Soul

* If Player has Unaware, Haze, Clear Smog, Freezy Frost, Topsy Turvy or a phazing move (and AI is not on last mon): -20 Score  
* If Player is incapacitated: +3 Score (90%)  
* Else if Player faints AI after setup: -2 Score (Accounts for berries)  
* Else +2 Score

<a id="acupressure"></a>
#### Acupressure

* If Player kills AI: -20 Score  
* If Player has Unaware, Haze, Clear Smog, Freezy Frost, Topsy Turvy or a phazing move: -20 Score  
* If Player fast kills AI in 2 hits: -5 Score (Accounts for Disguise)  
* If Player is incapacitated: +3 Score (90%)  
* Else if Player kills AI in 4 or more hits  
  * If Player is faster: +1 Score  
  * If Player is slower: +2 Score

<a id="charge"></a>
#### Charge

* If Player kills AI: -20 Score  
* If Player has a phazing move: -20 Score  
* If AI has an electric type move: +1 Score

<a id="defense-curl"></a>
#### Defense Curl  
Additional to the Defensive Setup properties:

* If AI has Rollout or Ice Ball, and AI doesn’t already have Defense Curl: +1 Score

<a id="stockpile"></a>
#### Stockpile  
Additional to the Defensive Setup properties:

* If AI has Spit Up or Swallow: +1 Score

<a id="fell-stinger"></a>
#### Fell Stinger  
If move can faint Player:

* If AI is faster: +9 Score  
* If AI is slower: +6 Score

<a id="meteor-beam-electro-shot"></a>
#### Meteor Beam, Electro Shot

* If move can be immediately used: +9 Score  
* Else -20 Score

<a id="sleep-sing-dark-void-yawn"></a>
#### Sleep (Sing, Dark Void, Yawn)  
25% of the time, if AI doesn’t see kill with its maxroll:

* If the target can be put to sleep: +1 Score  
* If it has the one of the following moves: Dream Eater, Nightmare, Snore, Sleep Talk: +1 Score  
* If it or the partner has the one of the following moves: Hex, Infernal Parade: +1 Score

Additionally, if it’s a Double Battle and the move is Dark Void: +2 Score (80%)

<a id="poison-poison-gas-toxic"></a>
#### Poison (Poison Gas, Toxic, etc.)   
20% of the time, if AI doesn’t see kill with its maxroll, and if the player’s HP is > 20%:

* If the player has no damaging moves: +1 Score  
* If AI has Protect, +1 Score  
* If AI has Venoshock, Hex, Infernal Parade, Venom Drench or Merciless: +1 Score

<a id="paralysis-nuzzle-thunder-wave-glare"></a>
#### Paralysis (Nuzzle, Thunder Wave, Glare, etc.)   
If AI doesn’t see kill with its maxroll:

* If AI is slower before paralysis but faster after paralysis: +2 Score  
* Else if AI has Hex, Infernal Parade or flinching moves: +2 Score  
* Else if Player is confused or infatuated: +2 Score  
* Else: +1 Score

<a id="burn-frostbite-sizzly-slide-will-o-wisp-freezy-frost"></a>
#### Burn, Frostbite (Sizzly Slide, Will-O-Wisp, Freezy Frost)   
33% of the time, if AI doesn’t see kill with its maxroll:

* +1 Score  
* If Player has physical moves (special moves for Frostbite): +1 Score  
* Else if AI or Partner has Hex or Infernal Parade: +1 Score

<a id="confusion-confuse-ray-supersonic-swagger-flatter"></a>
#### Confusion (Confuse Ray, Supersonic, Swagger, Flatter)   
25% of the time, if AI doesn’t see kill with its maxroll:

* If the target can be confused: +1 Score  
* If the player is paralyzed, infatuated or if the AI has Serene Grace and flinching moves: +1 Score

Additionally for Swagger and Flatter:

* If the AI has Psych Up, Spectral Thief, Mirror Herb or Foul Play (Swagger only): +1 Score  
* In a Double Battle, +9 Score (25%), +8 Score (75%) if the partner cannot be confused and if the partner benefits from the respective stat boost.

<a id="speed-lowering-effects"></a>
#### Speed lowering effects (Scary Face, Electroweb, Syrup Bomb, etc.)

* If AI is slower and move is status: +1 Score  
* If AI is faster: -2 Score

Additionally, if it’s a Double Battle and the move is a damaging spread move: +1 Score

<a id="attack-defense-special-defense-and-special-attack-lowering-effects"></a>
#### Attack, Defense, Special Defense and Special Attack lowering effects (Charm, Lunge, Screech, Rock Smash, Metal Sound, Lumina Crash, Confide, Mystical Fire, etc.)

* If Player has -1 of the stat or less: -2 Score (80%)  
* Else +1 Score (20%)  
* If move lowers Attack or Special Attack and Player doesn’t have a move of the corresponding category: -2 Score

<a id="accuracy-lowering-effects"></a>
#### Accuracy lowering effects  
80% of the time, if the player has -2 accuracy or less: -2 Score

* If AI HP > 90%, +2 Score (80%)  
* Else if AI HP > 60%, +1 Score (80%)  
* Else if AI HP < 60%, -1 Score

<a id="stealth-rock-stone-axe-spikes-ceaseless-edge-toxic-spikes-hazards"></a>
#### Stealth Rock, Stone Axe, Spikes, Ceaseless Edge, Toxic Spikes (Hazards)

* If Player is on last mon: -10 Score  
* If its AIs first turn and is not last mon: +2 Score (98%)  
* `0.75 * (AI Alive Mons / AI Total Mons)` of the time: +1 Score  
  * Example: If the AI has a total of 5 Pokémon and 3 are alive:
> `0.75 * (3 / 5)` = **45%** for **+1 Score**
* Additionally for (Toxic) Spikes: If there is 1 or more layers up: -1 Score (98%)

<a id="sticky-web"></a>
#### Sticky Web

* If Player is on last mon: -10 Score  
* If its AIs first turn: +3 Score  
* `0.75 * (AI Alive Mons / AI Total Mons)` of the time: +1 Score
  * Example: If the AI has a total of 5 Pokémon and 3 are alive:
> `0.75 * (3 / 5)` = **45%** for **+1 Score**

<a id="tailwind"></a>
#### Tailwind

* If Player has Trick Room or Taunt: -1 Score (50%)  
* If AI mon or its partner are slower than any player mon on the field: +3 Score  
* If Player has Tailwind up and Tailwind Setter is slower than target: +3 Score

<a id="trick-room"></a>
#### Trick Room

* If Player has Trick Room or Taunt: -1 Score (50%)  
* If AI mon or its partner are slower than any player mon on the field: +4 Score  
* Else: -1 Score

<a id="explosion-moves-memento"></a>
#### Explosion-Moves, Memento

| AI HP | Scoring |
| --- | --- |
| < 10% | +10 Score |
| < 33% | +8 Score (70%), +0 Score (30%) |
| < 66% | +7 Score (50%), +0 Score (50%) |
| Else | +7 Score (5%), +0 Score (95%) |

Additionally:

* If it’s the last mon for the AI  
  * If it isn’t the last mon for the player: -10 Score  
  * Else -1 Score  
* If the move is Memento and the target’s stats cannot be lowered: -20 Score

<a id="final-gambit"></a>
#### Final Gambit

* If AI mon is faster and has equal or higher current HP than player mon: +8 Score  
* If above is not true, and AI is faster and dies to player mon: +7 Score  
* Else:  +6 Score

Additionally:

* If it’s the last mon for the AI  
  * If it isn’t the last mon for the player: -10 Score  
  * Else -1 Score

<a id="baton-pass"></a>
#### Baton Pass

* If Player has a phazing move and AI has no stat raised: -20 Score  
* 25% of the time: -1 Score  
* If AI can pass something positive: +1 Score

<a id="u-turn-volt-switch-flip-turn-parting-shot"></a>
#### U-Turn, Volt Switch, Flip Turn, Parting Shot

* If AI is Palafin: +12 Score (doesn’t stack with anything else)  
* If AI kills Player in more than 3 hits: +6 Score (unless move is Parting Shots, which already starts as +6 Score due to being a status move)  
* If Player has a phazing move: -1 Score

<a id="knock-off"></a>
#### Knock Off

* If AI kills Player in more than 3 hits: +6 Score (Unless Player cannot lose the item)

<a id="screens-light-screen-reflect-aurora-veil"></a>
#### Screens (Light Screen, Reflect, Aurora Veil)  
If AI should set screen:

* +1 Score (50%)  
* If AI has Light Clay: +1 Score

AI fails the should set screen routine if the player has no physical move when Reflect is considered and vice versa. Aurora Veil always passes the check if snow or hail is active.

<a id="secret-power"></a>
#### Secret Power  
25% of the time, if Grassy Terrain is active: +6 Score

<a id="ohko-moves-fissure-horn-drill"></a>
#### OHKO Moves (Fissure, Horn Drill, etc.)

* If AI kills player in 3 or more hits: +6 Score  
* Else +5 Score  
* If Lock On is Active: +8 Score  
* If Player has Focus Band or Focus Sash/Sturdy active: -20 Score

<a id="binding-moves-fire-spin-whirlpool-snap-trap"></a>
#### Binding/Trapping Moves (Fire Spin, Whirlpool, Snap Trap, etc.)

* If player is immune to trapping: -20 Score  
* +6 Score (80%), +8 Score (20%)  
* If AI has Binding Band or Grip Claw: +1 Score

<a id="salt-cure"></a>
#### Salt Cure

* +6 Score (80%), +7 Score (20%)  
* If player is Water or Steel Type: +1 Score

<a id="trapping-octolock-mean-look-anchor-shot-spirit-shackle-thousand-waves-jaw-lock"></a>
#### Trapping (Octolock, Mean Look, Anchor Shot, Spirit Shackle, Thousand Waves, Jaw Lock, etc.)

* If player isn’t immune to trapping: +6 Score

<a id="recovery-moves-recover-slack-off-heal-order-roost-strength-sap-pain-split"></a>
#### Recovery Moves (Recover, Slack Off, Heal Order, Roost, Strength Sap, Pain Split, etc.)

* If AI decides it should recover: +1 Score  
* Else: -1 Score  
* Pain Split is only used if AI recovers more than 30%

For extra details on the function that AI uses to decide when to recover, see the extra details below.

<a id="drain-moves-giga-drain-draining-kiss"></a>
#### Drain-Moves (Giga Drain, Draining Kiss, etc.)  
If the target doesn’t have Liquid Ooze:

* If AI is at half HP or under, and if that move kills player in <= 4 hits: +6 Score  
* If AI has Big Root: +1 Score

<a id="copycat-mirror-move-me-first"></a>
#### Copycat, Mirror Move, Me First  
AI understands what move will be copied and applies its AI routine on it

<a id="roar-whirlwind"></a>
#### Roar, Whirlwind

* If AI has 3 layers of Spikes up: +1 Score  
* If AI has 2 layers of Spikes up: +1 Score (75%)  
* If AI has 1 layer of Spikes up: +1 Score (50%)  
* If AI has Stealth Rock up: +1 Score (50%)  
* 50% of the time: -1 Score

<a id="dragon-tail-circle-throw"></a>
#### Dragon Tail, Circle Throw

* If Player is Perish Song’ed: -20 Score  
* If Player can faint AI: -20 Score  
* Does not follow Roar AI.

<a id="conversion"></a>
#### Conversion  
+2 Score if type can still be changed.

<a id="conversion-2"></a>
#### Conversion 2

* If AI already resists or is immune to Players last used move: -20 Score  
* If Player can faint AI: +1 Score

<a id="laser-focus"></a>
#### Laser Focus

* If AI has Sniper: +1 Score  
* If target cannot be crit: -20 Score

<a id="focus-energy"></a>
#### Focus Energy

* If AI has Sniper, Super Luck, Scope Lens or High Crit Moves: +1 Score  
* If target cannot be crit: -20 Score

<a id="shed-tail"></a>
#### Shed Tail  
-20 if Player has sound moves or Infiltrator

* If Player can faint AI and AI is faster: +1 Score (50%)  
* Else: +1 Score (25%)

<a id="substitute"></a>
#### Substitute  
-20 if Player has sound moves (while AI doesn’t have Soundproof) or Infiltrator

* If Player has Perish Song effect: +1 Score  
* If Player is burned, poisoned or frostbitten: +1 Score (25%)  
* If Player is wrapped and AI HP > 70%: +1 Score (25%)  
* If AI has Speed Boost: +1 Score (25%)  
* 50% of the time: -1 Score

<a id="leech-seed"></a>
#### Leech Seed

* If Player doesn’t have Rapid Spin or Magic Guard: +1 Score (50%)  
* If AI kills Player in more than 3 hits: +1 Score (50%)

<a id="teleport-chilly-reception"></a>
#### Teleport, Chilly Reception

* If AI is faster and Player faints AI: -20 Score  
* If AI kills Player in more than 3 hits: +1 Score (50%)

<a id="sky-attack-freeze-shock-ice-burn"></a>
#### Sky Attack, Freeze Shock, Ice Burn

* If move can be immediately used: +9 Score (80%)  
* Else -20 Score

<a id="disable"></a>
#### Disable

* If AI is faster and last used move of player can faint AI: +1 Score

<a id="encore"></a>
#### Encore

* If AI is faster and last used move of player is encouraged to be encored: +1 Score  
* Encore encouraged effects: Status moves, Fake Out, First Impression

<a id="snore-sleep-talk"></a>
#### Snore, Sleep Talk

* If it’s not a wakeup turn and AI is asleep: +15 Score  
* Sleep Talk does not get a Score increase if the user has Comatose

<a id="destiny-bond"></a>
#### Destiny Bond

* If AI has Sash or Disguise active: -20 Score  
* If AI is faster and player can faint AI: +1 Score (81.5%)  
* Else if AI is slower: -1 Score (50%)

<a id="wish"></a>
#### Wish

* If any mon in Party has HP < 65%: +1 Score

<a id="aromatherapy"></a>
#### Aromatherapy

* If any mon in Party has status: +1 Score

<a id="nightmare"></a>
#### Nightmare

* If Player is asleep: +1 Score  
* If Player is trapped: +1 Score

<a id="perish-song"></a>
#### Perish Song

* If Player is trapped: +2 Score

<a id="weather-terrain-moves"></a>
#### Weather & Terrain Moves (Sunny Day, Sandstorm, Electric Terrain, etc.)

* +2 Score  
* If AI holds an item that increases its duration: +1 Score (80%)

<a id="attract"></a>
#### Attract

* If Player has any status or is trapped: +1 Score

<a id="taunt"></a>
#### Taunt

* If Player has a status move: +1 Score (50%)  
* Else: -1 Score (50%)

<a id="rollout-ice-ball"></a>
#### Rollout, Ice Ball

* +6 Score (50%), +7 Score (50%)  
* If AI has Defense Curl up: +1 Score

<a id="fury-cutter-echoed-voice"></a>
#### Fury Cutter, Echoed Voice

* +6 Score  
* If AIs last used move was Fury Cutter / Echoed Voice: +2 Score

<a id="protection-protect-kings-shield"></a>
#### Protection (Protect, King’s Shield, etc.)  
Protect, Detect, Spiky Shield, Silk Trap, King’s Shield, Baneful Bunker, Obstruct, Burning Bulwark

* If Player is incapacitated: -20 Score  
* If AI is about to faint at the end of the turn: -10 Score  
* If AI used a protection move the previous turn: -10 Score (50%)  
* If AI successfully used 2 protection moves in a row last turns: -10 Score

<a id="kings-shield-aegislash-ai"></a>
#### King’s Shield / Aegislash AI (doesn’t stack with the following parts of Protection AI)
* If Player is faster and can faint AI: +10 Score (80%)  
* If Player has physical moves: +1 Score (75%)  
* Else 37.5% of the time: +1 Score

<a id="power-construct-and-zen-mode-ai"></a>
#### Power Construct and Zen Mode AI
* If AI is in range of transforming, but not yet transformed: +8 Score (80%)

<a id="other-protection-logic"></a>
#### Other Protection Logic
* If AI has one of the following conditions: Burn, Poison, Curse, Infatuation, Perish Song, Leech Seed, Yawn: -1 Score  
* If Player has one of the above conditions outside of Infatuation: +1 Score  
* If AI has Speed Boost, is slower and is its first turn out: +3 Score (80%)  
* Else if its AIs first turn out, its not a Double Battle and doesn’t have one of the following combinations: Toxic/Flame Orb + Guts/Quick Feet, Flame Orb + Flare Boost: -1 Score

<a id="endure"></a>
#### Endure  
Endure uses the same counter as protection moves for failure checks

* If AI used a protection move the previous turn: -10 Score (50%)  
* If AI successfully used 2 protection moves in a row last turns: -10 Score  
* If Player can faint AI:   
  * If AI has one of the following: Pinch Berry, Flail, Reversal, Endeavor, Rage Fist: +2 Score  
  * Else if AI has Speed Boost: +1 Score, and an additional +1 Score if it also has Baton Pass  
  * Else: -1 Score (50%)  
* Else: -1 Score (50%)

<a id="fake-out"></a>
#### Fake Out

* +9 Score, stacks with HDM  
* If Player cannot be flinched and Fake Out doesn’t kill: -30 Score

<a id="feint"></a>
#### Feint

* If its a Double Battle and Player has a Protection move: +13 Score (10%)  
* Else if Feint can kill Player: +6 Score (10%)

<a id="upper-hand"></a>
#### Upper Hand

* If Player has a priority move: +13 Score (10%)

<a id="pursuit"></a>
#### Pursuit

* If AIs Ability is Truant or Defeatist and Players Ability is Mummy, Wandering Spirit or Lingering Aroma: +12 Score (Does not stack with the following)  
* If Move faints Player: +11 Score  
* Else if Players HP < 20%: +10 Score  
* Else if Players HP < 40%: +8 Score (50%)  
* If AI is faster: +3 Score

<a id="sucker-punch-thunderclap"></a>
#### Sucker Punch, Thunderclap

* If AI used Sucker Punch / Thunderclap last turn: -20 Score (66%)

<a id="imprison"></a>
#### Imprison

* If Player has moves that can be imprisoned: +3 Score

<a id="wonder-room"></a>
#### Wonder Room

* If Player has physical moves and AI has less defense than special defense (or vice versa): +1 Score  
* +2 Score (25%)

<a id="mud-sport-water-sport-magic-room"></a>
#### Mud Sport, Water Sport, Magic Room

* +3 Score (25%)

<a id="gravity"></a>
#### Gravity  
50% of the time

* +4 Score (75%), +5 Score (25%)

<a id="relic-song"></a>
#### Relic Song

* If AI is Meloetta: +10 Score  
* If AI is Meloetta-Pirouette: +1 Score (25%)

<a id="powder"></a>
#### Powder

* If Player has fire type moves: +1 Score  
* Else: -1 Score

<a id="magnet-rise"></a>
#### Magnet Rise

* If AI is faster and Player has Ground moves: +2 Score (90%)  
* Else: -1 Score

<a id="metronome"></a>
#### Metronome

* If its AIs last third (rounded down) of the team: -5 Score

<a id="fling"></a>
#### Fling

* If AI has King’s Rock and is faster and Player can be flinched: +9 Score  
* In a Double Battle on partner: If Fling uses Salac Berry:  
  * If it activates Weakness Policy: 12 Score (25%), +7 Score (75%)  
  * Else if partner is slower than any player mon on the field: +10 Score (25%), +8 Score (75%)  
  * Else: +8 Score (25%), +7 Score (75%)

<a id="topsy-turvy"></a>
#### Topsy Turvy

* If Players positive stat changes are higher than the negative stat changes: +1 Score  
* Else: -1 Score  
* In a Double Battle on partner: If Partners positive stat changes are lower than the negative stat changes: +10 Score (25%), +8 Score (75%)

<a id="revival-blessing"></a>
#### Revival Blessing  
AI always chooses first fainted mon in party order.

* +2 Score (50%)

<a id="counter"></a>
#### Counter

* If Player only has physical moves, can faint AI and AI has Focus Sash / Sturdy active: +2 Score  
* Else if Player only has physical moves: +2 Score (80%)  
* If AI is faster: -1 Score (25%)  
* If Player has a status move: -1 Score (25%)

<a id="mirror-coat"></a>
#### Mirror Coat

* If Player only has special moves, can faint AI and AI has Focus Sash / Sturdy active: +2 Score  
* Else if Player only has special moves: +2 Score (80%)  
* If AI is faster: -1 Score (25%)  
* If Player has a status move: -1 Score (25%)

<a id="metal-burst"></a>
#### Metal Burst

* If AI is faster than Player: -20  
* If AI has Focus Sash / Sturdy active: +2 Score  
* +1 Score (25%), If Player has a status move: -1 Score (50%)

<a id="psych-up-spectral-thief"></a>
#### Psych Up, Spectral Thief

* Loop through each stat  
  * If Players Atk stage is higher than AIs and AI has physical moves: +1 Score  
  * If Players Sp. Atk stage is higher than AIs and AI has special moves: +1 Score  
  * Unconditional +1 Score for every other stat  
* Psych Up on Partner in a Double Battle: If Partner has more raised stats: +10 Score (25%), +8 Score (75%)

#### Recharge  
Hyper Beam, Blast Burn, Hydro Cannon, Frenzy Plant, Giga Impact, Rock Wrecker, Roar of Time, Prismatic Laser, Meteor Assault, Eternabeam

* If move cannot faint player: -1 Score

#### Double Battle only

If the status move targets a partner, it does not get the base +6 Score by default.  
If the partner has one of the following abilities: +6 Score (25%) 

* Volt Absorb, Earth Eater, Water Absorb and Dry Skin (if HP <= 75%)  
* Lightning Rod, Storm Drain (if Sp. Atk can be increased and has special moves)  
* Sap Sipper (if Attack can be increased and has physical moves)  
* Motor Drive (if Speed can be increased)  
* Contrary

#### Priority Moves - Weakness Policy  
If priority move can activate Weakness Policy: +12 Score (25%), +8 Score (75%)

#### Spread Moves to override negative abilities (Brutal Swing)  
The following abilities count as a negative ability: Emergency Exit, Truant, Defeatist, Slow Start.  
If Partner is Mummy, Wandering Spirit or Lingering Aroma and move cannot faint partner: +9 Score (25%), +7 Score (75%)

#### Beat Up (Double Battle only)  
+9 Score (75%), +12 Score (25%) if:

* Partner has Justified / Scraftinite  
* Partner has physical moves and not raised attack stat  
* Beat Up cannot faint the partner  
* Partner is first turn out

#### Heal Pulse, Floral Healing, Pollen Puff  
If Partner is under half health and user is faster than both player mons: +6 Score

#### Helping Hand  
If Partner move is not a status move: +7 Score (50%)

#### Dragon Cheer

* +6 Score  
* If Partner is Dragon Type: +1 Score

#### Coaching  
50% of the time:

* +1 Score (50%)  
* If partner attack stat < +2: +1 Score (50%)  
* If partner defense stat < +2: +1 Score (50%)

#### Role Play  
If user doesn’t already have Huge Power or Pure Power and if partner has Huge Power, Pure Power or Illuminate: +10 Score (25%), +8 Score (75%)  

#### Entrainment  
If user has Huge Power and Partner doesn’t have Huge Power or Pure Power: +10 Score (25%), +8 Score (75%)

#### Teatime

* -1 Score (50%)  
* If user or partner has pinch berries: +8 Score  
* Else if user or partner has a berry: +6 Score

#### Instruct  
Starts at +6 Score and AI tries to evaluate the instructed move on the partner:

* If user is slower than partner, read the move the partner chose  
* If user is faster than partner, read the last used move of the partner

If the evaluated move isn’t a status move and a spread move: +1 Score (50%)

#### Acupressure, Speed Swap  
+8 Score (25%), +0 Score (75%)

#### Ally Switch  
20% of the time, if Player kills AI-Partner:

* If fast kill: +2 Score  
* If slow kill: +1 Score

#### Follow Me, Rage Powder  
If Player kills AI-Partner: +1 Score (50%)

#### Round

To understand Round AI, it is important to first understand how partner move scoring works in Double Battles.

Score calculations are processed sequentially. The AI first calculates all move scores for Slot 1 without knowledge of what Slot 2 will select. Slot 2 then calculates its scores afterward, while being fully aware of Slot 1’s chosen move and resulting score.

Round-specific scoring behaves as follows and stacks with HDM:

90% of the time, if the AI is faster and its partner has access to Round:

* +7 Score  
* The partner’s Round score is overridden to +13

!!! warning
    If the faster Round user is in Slot 1, the partner in Slot 2 has not yet calculated its scores at the time of the override. As a result, the override has no effect in this scenario.

If the AI is slower and its partner selects Round:

* The slower user receives a +13 score bonus.

!!! warning
    If the slower Round user is in Slot 1, it cannot yet know whether Slot 2 will choose Round, since Slot 2 has not performed its calculations yet. To compensate for this limitation, the previously mentioned score override is applied instead.