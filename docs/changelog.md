# Changelog

This page records notable changes, fixes, and balance updates for Pokémon Null.

## Version 1.2.6

### Bug fixes

- Fixed Mega Evolutions sometimes being unable to move.
- Fixed Delphox not being able to learn Psystrike.
- Fixed Lottery being redoable if you do not speak to the Clear a second time.
- Fixed several move effects not working correctly, including Alluring Voice, Anchor Shot, and Spirit Shackle.
- Fixed Struggle failing on Prankster when all usable moves are priority moves.

## Version 1.2.5

### Bug fixes

- Fixed several issues with Berries that apply stat changes.
- Fixed Silk Trap, Obstruct, Burning Bulwark, Mat Block, and Crafty Shield incorrectly blocking Status Moves.
- Fixed Covert Cloak not working against abilities and items that add additional effects, such as King's Rock and Poison Point.
- Fixed Powder affecting Grass-Types.
- Fixed Glaive Rush missing its Contact property.
- Fixed Flare Blitz not being boosted by Reckless.
- Fixed Terrain Pulse not applying its effect when the user is not grounded.
- Fixed Persim Berry having a delayed activation when Outrage confuses.
- Fixed Adrenaline Orb not activating when Intimidate is blocked by Clear Body.
- Fixed Intimidate and similar abilities triggering Eject Pack at the wrong time when Mega Evolving.
- Fixed Greta being unable to set Stealth Rock with Stone Axe.
- Fixed the pond in Rustboro Grove being walkable on some tiles.

### AI fixes and adjustments

- Fixed AI being able to use Stone Axe or Ceaseless Edge when Stealth Rock or Spikes, respectively, are already maxed out.
- Fixed AI being able to use Stone Axe or Ceaseless Edge over fast kill when it isn't intended.
- Fixed AI incorrectly using Syrup Bomb when it shouldn't, such as against Clear Amulet.
- Fixed AI incorrectly calculating Revenge as boosted when it shouldn't during switch-in evaluation.
- Fixed AI applying a score penalty to self-targeting moves when the target is in a semi-vulnerable state and the AI is faster.
- Fixed AI not correctly applying a score penalty to setup moves in certain cases, such as Take Heart and Stuff Cheeks when facing Unaware.
- Fixed AI evaluating Stomping Tantrum at full power during switch-in evaluation if the previous Pokémon was flinched.
- Fixed AI being able to use Memento against targets with Clear Body or White Smoke.
- Fixed AI incorrectly applying a Gem boost to Future Sight, which cannot be boosted by Gems.
- Fixed Feint AI not applying if the target has Wide Guard or Quick Guard alongside a Protection Move.
- Fixed some Shell Smash setup discouragement checks not being properly applied by the AI.
- Fixed Upper Hand AI having the wrong percentage of being used.
- Fixed King's Shield AI incorrectly applying to Aegislash-Shield.
- Removed Two-Turn AI to eliminate some unwanted side effects. Sky Attack, Freeze Shock, and Ice Burn are now calculated like regular damage, but are still discouraged by AI when no Power Herb is present.

### Learnsets

- Fixed some oversights where Pokémon were missing moves due to their evolution level, including Armaldo missing Rock Blast and Kingdra missing Icy Wind.
- Metal Burst and Counter are now Heart Scale exclusive moves for Archaludon.
- Added Level 99 and/or Level 100 moves for some of the weaker Safari Zone Pokémon, Ultra Beasts, and a few other Pokémon (e.g Luxray, Goodra, Ursaluna-Bloodmoon).
- Slightly improved the learnsets of some future Paradox Pokémon.
- Some other minor changes may have been made but are not further specified.

### Trainers

- Reduced the Level of the following Pokémon by 1: Camper Charlie's Floette-Eternal, Fallarbor Courtney's Iron Moth.
- Reworked Blackbelt Nob's Conkeldurr for consistency reasons: Conkeldurr is no longer preburned and now has Flame Orb.
- Slightly reduced the amount of Hurricanes in the game: Ninja Boy Lao Noctowl Hurricane -> Air Slash and Gym Leader Winona 1 Celesteela Hurricane -> Air Slash.
- Gym Leader Winona 1's Landorus: Floaty Fall -> Fly.
- Magma Grunt Zeldest's Yveltal has been reworked: Fiery Wrath -> Dark Pulse, Black Glasses -> Apicot Berry.
- Seafloor Cavern Archie's Iron Jugulis: Yache Berry -> Assault Vest to improve Iron Bundle's viability for the fight.
- Triathlete Stephin's Ogerpon: Growth -> Upper Hand to remove some severe cheese.
- John & Jay's Iron Jugulis: Terrain Pulse -> Thunderbolt to account for the above bugfix.
- Pokéfan Bethany's Chi Yu: Energy Ball -> Ruination.
- Changed Juan's Kingdra set to account for Electric Terrain being permanent since 1.2, which made its Chesto Berry Rest set no longer work.
- Rocket Ambush Weezing: Focus Band -> Ability Shield to make the fights less restrictive.
- Youngster Des' Blaziken: Bolt Strike -> Thunder Punch.
- Slightly changed the Maxie & Archie Double Battle in Victory Road based on community feedback.
- Nature mistakes: MHO Grunt #10's Zarude: Timid -> Jolly, SFC Shelly's Pheromosa: Naive -> Jolly.
- As compensation for some of the above nerfs, to keep a similar overall difficulty, the following sets have been buffed: Sis And Bro Reli&Ian's Kricketune, Leaf 2 Deoxys, Frontier Head Noland's Mawile.

### Other

- The following tables have been adjusted: Route 111 Static, Route 119, Magma Hideout 1F.
- Slowking Ability: Shell Armor -> Regenerator. For compensation, an Ability Tutor is included in Dewford Town that turns Slowking's Ability into Shell Armor for 3 Scales.
- Reverted Hurricane to being a Wind move following community feedback.
- Added a new Move Tutor in Sootopolis City to provide more flexibility when building lategame movesets. Also added Heal Bell and Aromatherapy to the Route 120 Move Tutor, and Air Cutter to the second Petalburg Move Tutor.
- Added a comeback mechanic for struggling Nuzlocke runs to encourage keep playing bleeding runs. See the Mechanic Changes document for details.
- Adjusted the Elite Four Heart Scale Shop to lower prices, remove redundant items, and introduce new ones. Most notably, added the Recall Charm, which allows a Pokémon to relearn a move upon use.
- Added TM22 Poison Jab to Route 118, as it was previously unavailable outside of the Lilycove Department Store.
- Added Hidden Ability Tutors for the following Pokémon: Tauros-Paldea-Combat, Amoonguss, Hatterene, Toxapex, Hydrapple, Slowbro, Cyclizar.
- Added an NPC in Lilycove City Contest Hall that gives you an Air Balloon after the 7th Badge if Spinda is shown.
- Added an NPC on Route 111, past the Desert, who gives you an Ability Capsule if you show her a Pokémon with an RNG based ability (such as Flame Body) and an alternative ability, provided it currently has the RNG based ability.
- Added the Return All Items feature to the Gauntlet menu.
- Added a quality of life feature that lets you change Shoal Cave's state.
- Reduced Golisopod's catch rate from 15 to 1.
- Wild Ultra Beasts now hold Berserk Gene.
- Improved Morty's and Clair's themes. (Credits to IAGeezus.)

## Version 1.2.4

### Bug fixes

- Fixed Good as Gold blocking Curse from non Ghost type Pokémon.
- Fixed Dragon Tail's effect working on Mimikyu with Disguise active.
- Fixed Dark types incorrectly being immune to Struggle from Prankster Pokémon if they had a status move.
- Fixed eject activation (Emergency Exit and Eject items) incorrectly passing the endure effect.
- Fixed Stomping Tantrum not being boosted if the previous move missed because the target was in a semi invulnerable state.
- Fixed Stomping Tantrum remaining boosted for the rest of the battle after activating from a miss, which also caused the AI to overvalue it when evaluating switch ins.
- Fixed Covert Cloak incorrectly blocking Silk Trap and Obstruct effects if the triggering move would be blocked by Covert Cloak.
- Fixed a softlock occurring when viewing an Egg summary screen.
- Fixed Defog being used by the target instead when they are behind a Substitute while Reflect or Light Screen is active.
- Fixed Tera Starstorm not being boosted by Sheer Force, which also caused Covert Cloak and Shield Dust to fail to block its effect.
- Fixed Supersweet Syrup and Illuminate incorrectly activating Adrenaline Orb.
- Fixed a visual bug with Tar Shot displaying a failure message when the target was already affected by Tar Shot but its Speed could still be lowered.
- Fixed Wallace's Diancie's Mega Evolution not cancelling multihit moves as intended.
- Fixed Binding Move score stacking with HDM.
- Fixed Echoed Voice and similar moves not resetting their stack boost after a flinch and similar interruptions.
- Fixed the Quality of Life menu missing the Air Slash and Signal Beam tutors.
- Fixed Last Resort not working properly when previous moves were interrupted before being used).
- Fixed Struggle recoil not using standard rounding.
- Fixed the AI incorrectly applying Technician to a boosted Payback.
- Fixed Mortal Spin's spinning effect activating even when hitting an immune target.
- Fixed Focus Sash reactivating after being consumed by Future Sight.
- Fixed Zoom Lens activating if the original target switched out using a pivot move.
- Fixed Fling effects not activating if the target's held item activated during the attack (e.g. Focus Sash, Colbur Berry).
- Fixed Teatime not affecting certain Pokémon in double battles depending on their position.
- Fixed Wandering Spirit not transferring if Pursuit hit a Pokémon using a pivot move.
- Fixed Wandering Spirit incorrectly working on Protosynthesis and Quark Drive.
- Fixed Sleep Talk and Snore not properly reducing sleep turns when switching out.
- Fixed contact draining moves (Draining Kiss and Drain Punch) being able to heal through Spiky Shield.
- Fixed Gulp Missile damage incorrectly corrupting the healing amount of moves such as Giga Drain.
- Fixed Salac Berry and similar effects triggering their animation without properly applying the Speed boost, instead causing the opponent to receive the boost.
- Fixed Life Orb recoil not happening when a move hits but deals no damage (e.g. due to Endure or Ice Face).
- Fixed Jaboca Berry and similar effects not activating when breaking Eiscue's Ice Face.
- Fixed Cotton Down incorrectly ending multihit moves when the target's Speed could not be lowered further.
- Fixed Pursuit causing the game to crash when targeting a Pokémon with Cotton Down that attempts to switch out.
- Fixed a crash when the Player used Me First and the AI is considering Mirror Move.
- Fixed a crash in the Player PC when withdrawing a Berry.
- Fixed Fling incorrectly using the held TM's base power when a Pokémon holding a TM used Fling.
- Fixed Matcha Gotcha not thawing a frozen target.
- Fixed Flare Blitz being able to burn a target after thawing it.
- Fixed Perish Body not activating when the Pokémon was KO'd.

### AI fixes

- Fixed AI being able to see the player's remaining PP. (The AI can still see its own PP.)
- Fixed AI sometimes being able to use OHKO moves against targets with Focus Band.
- Fixed AI seeing the full damage of Rollout and similar moves on the first turn and when evaluating switches.
- Fixed AI applying Technician to every hit of Fury Cutter and similar moves.
- Fixed AI applying the wrong score to Order Up and OHKO moves.
- Fixed AI using Mirror Move and Copycat on the first turn and when no move can be copied yet.
- Fixed AI using Entrainment against a target holding an Ability Shield.
- Fixed AI sometimes seeing Last Resort damage when evaluating switch ins.
- Fixed AI being able to use Memento when it was down to its last Pokémon.
- Fixed AI incorrectly seeing the Stakeout boost after a pivot move KO.
- Fixed AI using damaging setup moves like Power-Up Punch despite the player being slower and guaranteeing a KO.
- Fixed AI not using semi invulnerable moves if it incorrectly expected to die to sandstorm or hail chip.
- Fixed AI not accounting for Ability suppression on certain defensive Abilities, such as Marvel Scale and Fur Coat.
- Fixed AI incorrectly applying a score penalty to Ditto during switch-in evaluation when it could be fast KO'd.
- Fixed AI treating the next switch in as if its Ability were disabled after a Pokémon fainted under the effect of Gastro Acid.
- Fixed AI calculating moves like Endeavor and Counter as dealing 1 damage, along with other minor inconsistencies when evaluating these moves.
- Fixed AI using Swords Dance with Mimikyu while Disguise is intact, even when the opponent has a move that discourages setup, such as Haze.
- Fixed Counter Tailwind AI activating after the player's Tailwind had already ended.
- Removed Truant AI because it was buggy.

### AI changes

- Acupressure can now be discouraged by showing a fast 2HKO.

### Balance

- Poison Fang BP: 50 -> 65 to make early Boltund and Drapion better.
- Zippy Zap PP: 10 PP -> 1 PP, Silk Trap PP: 5 PP -> 1 PP.
- Drampa Ability: Berserk -> Thick Fat, Hidden Ability: Sap Sipper -> Berserk, Stunfisk Ability: Limber / Sand Veil -> Own Tempo.
- Improved the learnsets of the following Pokémon: Luxray, Delcatty, Persian, Masquerain, Raichu-Alola, Boltund, Eldegoss, Drampa, Armaldo, Amoonguss, Rapidash-Galar, and Swanna. These changes provide small buffs without significantly altering their power level.
- Changed Leavanny's moveset to make its Sharpness variants slightly weaker and its Leaf Guard variants slightly better.
- Delphox now gets Mist Ball instead of Recycle via Heart Scale and Luster Purge at Level 100, to add synergy with Serene Grace Mega Delphox. As compensation, Greninja and Chesnaught also received respectively Storm Throw and Horn Leech at Level 100.
- Added Lucky Chant, Psychic Noise, Counter and Mirror Coat to the learnsets of some Pokémon, as these moves were previously underrepresented.
- Made a few additional learnset adjustments for consistency, move repeats, vanilla accuracy, and to replace level up moves that were already available via tutors. (For example, Obstagoon now learns Return via TM, Coalossal now learns Lucky Chant instead of Rock Slide at Level 58.)
- Cooltrainer Marcel's Hitmontop now holds a Coba Berry instead of a Muscle Band to compensate for a miscalculation involving the interaction between Quick Draw and Mega Evolution.
- Reduced the levels of the following Pokémon by 1: Breeder Tommy's Zangoose, Land Cave Elite Grunt's Nidoqueen, School Kid Mewttin's Goodra and MHO Grunt Zeldest's Yveltal.
- As compensation for these nerfs, a few minor changes have been made starting from Steven Split. Most notably, Shelly's Ceruledge in SFC now holds a Colbur Berry instead of Heavy-Duty Boots and Juan's Iron Bundle now has Terrain Pulse instead of Flip Turn.
- Roxanne's Aerodactyl now has a Special Attack IV of 4 to slightly improve Armaldos matchup against it.
- Lady Cindy's Delcatty now has Snore and Twins Gina&Mia's Leafeon now has Absorb. These changes eliminate them as Support Pokémon.
- Reshiram in MHO now has Minimize instead of Double Team to enable Dragon Rush strategies.
- Moveset nerfs for the following Pokémon in Root Academy: Wooloo, Clamperl, Rockruff, Hatenna, Flabébé.
- Added a Rock Smash encounter in Fiery Path to give Nuzlocke players an option to avoid encountering Heatmor. The following Pokémon can now be encountered: Magmortar, and Electivire, Lycanroc-Day, Ampharos, Pyroar.
- Added Water encounters to Rustboro Grove to give the option to opt out from a high variance table.
- Added Purrloin to Rustboro Grove and instead made Luxio slightly rarer.
- Zippy Zap is now exclusive to Pichu. Rustboro Grove's Pikachu has been replaced with Pichu to prevent early access via Mauville City Pikachu.
- Slowpoke now evolves randomly into Slowbro or Slowking. The movesets of both Slowbro and Slowking have been adjusted accordingly.

### Items

- Wild Bergmite now hold Ice Stone.
- Wild Gulpin and Swalot now hold Iapapa Berry.
- Wild Skitty and Delcatty now hold King's Rock.
- Wild Glameow and Purugly now hold Adrenaline Orb.
- Slowbroite is now available in Mossdeep Gym instead of Route 134.

### Other

- Replaced Experts Ronald and Makayla with Tourists Morty and Clair for a more climactic experience. Their teams remain unchanged.
- Added Courtney and Zinnia cutscenes on Route 111 and in Sky Pillar, respectively.
- Added the Return All Items feature to the Misc Menu.

## Version 1.2.3

### Fixes

- Adjusted the three Finizen in the Finizen Fanclub so they now only use Sonicboom.
- Fixed an issue where the Air Slash and Signal Beam tutors were not functioning as intended.
- Fixed a bug where a placeholder species could be encountered while fishing on Route 124.
- Fixed a Belly Drum AI logic issue involving post-Belly Drum survival.
- Fixed various Covert Cloak and Shield Dust interactions.
- Fixed Stomping Tantrum not receiving its power boost when a move failed due to an immunity-granting Ability that raises stats.
- Fixed a rounding error affecting Protean and Libero.
- Fixed an issue with Sticky Barb being duplicated.
- Fixed Me First only copying the first hit of multi-hit moves.
- Fixed various issues involving Mycelium Might.
- Fixed Dipplin's icon missing its animation.

## Version 1.2.2

### AI fixes

- Removed AI consideration of Zap Cannon when spreading paralysis through Nuzzle AI.
- Fixed Fake Out KOs being discouraged against targets that cannot be flinched.
- Fixed Metal Burst not receiving its baseline score.
- Fixed Magnet Rise AI incorrectly evaluating the player's Electric-type moves instead of Ground-type moves.
- Fixed an incorrect percentage in the Round AI logic.
- Fixed AI using Focus Energy and Laser Focus against targets that are immune to critical hits.
- Fixed Stockpile AI score increases being applied twice.
- Fixed errors in hazard AI logic when the AI was on its last remaining Pokémon.
- Fixed inconsistencies with Feint AI logic and Hyperspace Hole discouragement.
- Fixed Salt Cure and Syrup Bomb score penalties being applied when the user was affected instead of the target.

### Bug fixes

- Fixed an issue where using a Tutor would sometimes result in a Pokémon losing levels.
- Fixed Mighty Cleave incorrectly removing the effects of protection moves.
- Fixed frozen Pokémon taking crash damage.
- Fixed Pain Split not being treated as passive damage.
- Fixed Symbiosis activating when an Eject item was consumed.

### Hotfixes

- Replaced Slowking's Yawn with Hypnosis and added Yawn as a Scale Move.
- Replaced Slowbro's Heal Pulse with Extrasensory.
- Replaced Chip Away with Aqua Cutter in Feraligatr's learnset.
- Added several new learnset improvements to Grafaiai, Arbok, and other Pokémon.
- Adjusted several abilities, including Tornadus-Therian and Tangela.
- Added Sky Uppercut to several learnsets.

### Quality of life

- Casual Mode now provides 200 Heart Scales instead of 50.
- Added Revive to Oldale Town mart.
- Added a Return All Items feature.
- Increased the Poké Ball catch rate modifier from 1× to 1.5×.
- Added Fly points at Mt. Pyre Summit and Route 128.
- Added a new post-Maxie cutscene in Magma Hideout.

### Other

- Added Signal Beam and Air Slash as tutor moves in Route 120.
- Added OHKO moves to the Avoid Switch condition for midturn switch AI.
- Adjusted Gloom's moveset in Root Academy.
- Removed a duplicate Sentret from Root Academy.
- Reduced specific IVs for several Root Academy Pokémon.
- Renamed Camper Derek on Route 111 to Camper Tanjiro.

## Version 1.2.1

### Aesthetics

- Updated several sprites and icons for improved quality.
- Added shiny sprites for the Mega Evolutions introduced in Pokémon Legends: Z-A.

### Learnset changes

- Adjusted moveset repeats, swaps, additions, and other changes for several Pokémon.
- Added Hidden Power to the learnset of Generation 7+ Pokémon and corrected several learnset inconsistencies.

### Bugs

- Fixed a final Surf encounter slot issue.
- Fixed AI retaining Ability and Item data after a KO and pivot move interaction.
- Fixed Absorb, Recoil, and Rapid Spin effects failing to trigger when hitting a Substitute.
- Fixed AI choosing the wrong switch-in candidate after Eject Button activation.
- Fixed AI mid-turn switching into a dead Pokémon in specific circumstances.
- Fixed AI using Shell Smash in unintended scenarios.
- Fixed moves like Echoed Voice increasing in base power even if they failed.
- Fixed Throat Chop lasting indefinitely.
- Fixed non-Tri Attack variants of Nature Power being affected by abilities such as Refrigerate.
- Fixed Mega Evolution and transformed Pokémon state issues.
- Fixed Coaching succeeding in semi-invulnerable states.
- Fixed status immunity and protection move interactions.
- Fixed various issues involving Protect, Baneful Bunker, Clear Amulet, and Protective Pads.
- Fixed Population Bomb and Iron Barbs interaction issues.
- Fixed Water Shuriken damage issues for Ash-Greninja.
- Fixed Encore interaction issues after a Pokémon was unable to move.

### Other

- Reverted Blaziken's Ability to its previous version.
- Added a Speed Boost tutor.
- Corrected Pyre Team Aqua Grunt #3's Rotom nature.
- Adjusted several IVs.
- Replaced Probopass with Duraludon in the Navel Rock Sturdy Table.
- Removed the Focus Energy Tutor from the L-Menu.
- Reverted the Jagged Pass met location name.
- Replaced Wally's Zigzagoon with Galarian Zigzagoon.
- Improved Pokédex search functionality.

### AI changes

- Reduced support Pokémon switch score boosts to 10%.
- Removed Future Sight Switch-AI due to bugs.
- Adjusted several midturn switch parameters to be slightly more lenient.

## Version 1.2.0

### Overall changes

- Adjusted several learnsets, trainers, abilities, and encounter tables.
- Added a new trainer battle in Steven Split.
- AI Pokémon now have maxed PP in all moves; moves with 1 base PP for the player default to 8 PP for the AI.
- Candy Jar and Common Candy can no longer be registered.

### Move-related changes

- Adjusted several move effects, accuracy values, power values, and PP values.
- Various mechanic changes were made to moves such as Obstruct, Tera Starstorm, Aeroblast, Water Shuriken, Hurricane, and more.
- Several Tutors and item locations were adjusted.

### Item-related changes

- All resist berries now yield 1.
- PP Up is no longer available in Meteor Falls.
- Tyranitarite location changed to Sky Pillar.
- Several item locations and trade restrictions were changed.

### AI-related changes

- Adjusted mid-turn Switch AI to account for PP stalling strategies.
- Added additional AI checks to recognize conditions such as possible KO scenarios and other evaluation edge cases.

