# Changelog

This page records notable changes, fixes, and balance updates for Pokémon Null.

## Version 1.2.6

### Bug fixes

- Fixed Mega Evolutions sometimes being unable to move.
- Fixed Delphox not being able to learn Psystrike.
- Fixed Lottery being redoable if you do not speak to the Clear a second time.
- Fixed several move effects not working correctly, including Alluring Voice, Anchor Shot, and Spirit Shackle.
- Fixed Struggle failing on Prankster when all usable moves are priority moves.

### AI fixes

- Fixed the AI being able to see the player's remaining PP. The AI can still see its own PP.
- Fixed AI sometimes being able to use OHKO moves against targets with Focus Band.
- Fixed AI seeing the full damage of Rollout and similar moves on the first turn and while evaluating switches.
- Fixed AI applying Technician to every hit of Fury Cutter and similar moves.
- Fixed AI applying the wrong score to Order Up and OHKO moves.
- Fixed AI using Mirror Move and Copycat on the first turn or when no move can yet be copied.
- Fixed AI using Entrainment against a target holding an Ability Shield.
- Fixed AI sometimes seeing Last Resort damage while evaluating switch-ins.
- Fixed AI being able to use Memento when it was down to its last Pokémon.
- Fixed AI incorrectly seeing the Stakeout boost after a pivot move KO.
- Fixed AI using damaging setup moves like Power-Up Punch even when the player is slower and guaranteed to KO.
- Fixed AI not using semi-invulnerable moves if it incorrectly expected to die from sandstorm or hail chip.
- Fixed AI not accounting for Ability suppression on defensive Abilities like Marvel Scale and Fur Coat.
- Fixed AI incorrectly applying a score penalty to Ditto during switch-in evaluation when it could be fast KO'd.
- Fixed AI treating the next switch-in as though its Ability were disabled after a Pokémon fainted under Gastro Acid.
- Fixed AI calculating moves like Endeavor and Counter as dealing 1 damage and other minor evaluation inconsistencies.
- Fixed AI using Swords Dance with Mimikyu while Disguise is intact, even when the opponent has a discouraging move like Haze.
- Fixed Counter Tailwind AI activating after the player's Tailwind had already ended.
- Removed Truant AI because it was buggy.

### AI changes

- Acupressure can now be discouraged by showing a fast 2HKO.

### Balance

- Poison Fang base power: 50 → 65.
- Zippy Zap PP: 10 → 1.
- Silk Trap PP: 5 → 1.
- Drampa ability changes were adjusted, and several learnsets were improved for a number of Pokémon, including Luxray, Delcatty, Persian, Masquerain, Raichu-Alola, Boltund, Eldegoss, Drampa, Armaldo, Amoonguss, Rapidash-Galar, and Swanna.
- Leavanny's Sharpness variants were slightly weakened, while its Leaf Guard variants were improved.
- Delphox now learns Mist Ball instead of Recycle via Heart Scale and Luster Purge at level 100, with corresponding compensation for Greninja and Chesnaught.
- Lucky Chant, Psychic Noise, Counter, and Mirror Coat were added to the learnsets of some Pokémon.
- Several additional learnset adjustments were made for consistency, move repeats, accuracy, and to replace level-up moves already available via tutors.
- Cooltrainer Marcel's Hitmontop now holds a Coba Berry instead of a Muscle Band.
- The levels of several trainer Pokémon were reduced by 1.
- Several trainer teams and encounters received minor revisions, including a few Root Academy move-set changes, encounter adjustments in Fiery Path and Rustboro Grove, Purrloin additions, and Slowpoke evolution changes.

### Item and encounter updates

- Wild Bergmite now hold Ice Stone.
- Wild Gulpin and Swalot now hold Iapapa Berry.
- Wild Skitty and Delcatty now hold King's Rock.
- Wild Glameow and Purugly now hold Adrenaline Orb.
- Slowbroite is now available in Mossdeep Gym instead of Route 134.
- A Rock Smash encounter was added in Fiery Path.
- Added Water encounters to Rustboro Grove.
- Added Purrloin to Rustboro Grove and reduced Luxio's appearance rate.
- Zippy Zap is now exclusive to Pichu, and Rustboro Grove's Pikachu was replaced with Pichu.
- Slowpoke now evolves randomly into Slowbro or Slowking.

### Other changes

- Replaced Experts Ronald and Makayla with Tourists Morty and Clair.
- Added Courtney and Zinnia cutscenes on Route 111 and Sky Pillar.
- Added the Return All Items feature to the Misc Menu.

## Version 1.2.5

### Bugs

- Fixed several issues with berries that apply stat changes.
- Fixed Silk Trap, Obstruct, Burning Bulwark, Mat Block, and Crafty Shield incorrectly blocking status moves.
- Fixed Covert Cloak not working against abilities and items that add additional effects, such as King's Rock and Poison Point.

## Version 1.2.4

### Bug fixes

- Fixed Good as Gold blocking Curse from non-Ghost-type Pokémon.
- Fixed Dragon Tail's effect on Mimikyu with Disguise active.
- Fixed Dark types incorrectly being immune to Struggle from Prankster Pokémon if they had a status move.
- Fixed eject activation incorrectly passing the endure effect.
- Fixed Stomping Tantrum not being boosted if the previous move missed because the target was in a semi-invulnerable state.
- Fixed Stomping Tantrum remaining boosted after activating from a miss.
- Fixed Covert Cloak incorrectly blocking Silk Trap and Obstruct effects when the triggering move would have otherwise been blocked by Covert Cloak.
- Fixed a softlock when viewing an Egg summary screen.
- Fixed Defog being used by the target instead when behind a Substitute while Reflect or Light Screen is active.
- Fixed Tera Starstorm not being boosted by Sheer Force.
- Fixed Supersweet Syrup and Illuminate incorrectly activating Adrenaline Orb.
- Fixed a visual bug with Tar Shot displaying a failure message when the target was already affected.
- Fixed Wallace's Diancie's Mega Evolution not cancelling multihit moves as intended.
- Fixed Binding Move score stacking with HDM.
- Fixed Echoed Voice and similar moves not resetting their stack boost after a flinch.
- Fixed Last Resort not working properly when previous moves were interrupted before being used.
- Fixed Struggle recoil not using standard rounding.
- Fixed the AI incorrectly applying Technician to a boosted Payback.
- Fixed Mortal Spin's spinning effect activating even when hitting an immune target.
- Fixed Focus Sash reactivating after being consumed by Future Sight.
- Fixed Zoom Lens activating if the original target switched out using a pivot move.
- Fixed Fling effects not activating if the target's held item activated during the attack.
- Fixed Teatime not affecting certain Pokémon in double battles depending on position.
- Fixed Wandering Spirit not transferring if Pursuit hit a Pokémon using a pivot move.
- Fixed Wandering Spirit incorrectly working on Protosynthesis and Quark Drive.
- Fixed Sleep Talk and Snore not properly reducing sleep turns when switching out.
- Fixed contact draining moves being able to heal through Spiky Shield.
- Fixed Gulp Missile damage incorrectly corrupting healing amounts.
- Fixed Salac Berry and similar effects triggering their animation without properly applying the Speed boost.
- Fixed Life Orb recoil not happening when a move hits but deals no damage.
- Fixed Jaboca Berry and similar effects not activating when breaking Eiscue's Ice Face.
- Fixed Cotton Down incorrectly ending multihit moves when the target's Speed could not be lowered further.
- Fixed Pursuit causing a crash when targeting a Pokémon with Cotton Down that attempts to switch out.
- Fixed a crash when the Player used Me First and the AI was considering Mirror Move.
- Fixed a crash in the Player PC when withdrawing a Berry.
- Fixed Fling incorrectly using the held TM's base power when a Pokémon holding a TM used Fling.
- Fixed Matcha Gotcha not thawing a frozen target.
- Fixed Flare Blitz being able to burn a target after thawing it.
- Fixed Perish Body not activating when the Pokémon was KO'd.

### AI fixes

- Fixed AI being able to see the player's remaining PP.
- Fixed AI sometimes being able to use OHKO moves against targets with Focus Band.
- Fixed AI seeing the full damage of Rollout and similar moves on the first turn and when evaluating switches.
- Fixed AI applying Technician to every hit of Fury Cutter and similar moves.
- Fixed AI applying the wrong score to Order Up and OHKO moves.
- Fixed AI using Mirror Move and Copycat on the first turn and when no move can yet be copied.
- Fixed AI using Entrainment against a target holding an Ability Shield.
- Fixed AI sometimes seeing Last Resort damage when evaluating switch-ins.
- Fixed AI being able to use Memento when it was down to its last Pokémon.
- Fixed AI incorrectly seeing the Stakeout boost after a pivot move KO.
- Fixed AI using damaging setup moves like Power-Up Punch despite the player being slower and guaranteeing a KO.
- Fixed AI not using semi-invulnerable moves if it incorrectly expected to die to sandstorm or hail chip.
- Fixed AI not accounting for Ability suppression on certain defensive Abilities, such as Marvel Scale and Fur Coat.
- Fixed AI incorrectly applying a score penalty to Ditto during switch-in evaluation when it could be fast KO'd.
- Fixed AI treating the next switch-in as if its Ability were disabled after a Pokémon fainted under Gastro Acid.
- Fixed AI calculating moves like Endeavor and Counter as dealing 1 damage, along with other minor inconsistencies.
- Fixed AI using Swords Dance with Mimikyu while Disguise is intact, even when the opponent has a move that discourages setup, such as Haze.
- Fixed Counter Tailwind AI activating after the player's Tailwind had already ended.

### AI changes

- Removed Truant AI because it was buggy.

### Balance

- Poison Fang base power: 50 → 65.
- Zippy Zap PP: 10 → 1.
- Silk Trap PP: 5 → 1.
- Drampa's ability and hidden ability were adjusted, and several Pokémon learnsets were improved.
- Delphox now learns Mist Ball instead of Recycle via Heart Scale and Luster Purge at level 100.
- Added Lucky Chant, Psychic Noise, Counter, and Mirror Coat to select learnsets.
- Several additional learnset tweaks were made for consistency and balance.

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

