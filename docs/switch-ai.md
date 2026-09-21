# Switch AI

## Post-KO Switch AI Scores

When the AI needs to switch in a Pokémon (after a faint or similar event), it calculates a switch-in score for each of its Pokémon against the player's active Pokémon. It will then send out the Pokémon with the highest score. In case of ties, it selects the first Pokémon in party order.  
In *Double Battles*, each slot is evaluated independently: 

* The AI’s first slot evaluates against the player’s first slot  
* The AI’s second slot evaluates against the player’s second slot 

| Score | Condition |
| --- | --- |
| +5 | AI's Pokémon is faster than the player's and OHKOs it. | 
| +4 | AI's Pokémon is slower than the player's and OHKOs it. Or AI considers Palafin-Zero. |
| +3 | AI's Pokémon is faster than the player's and KOs in <= hits. Or AI considers Imposter Ditto. |
| +2 | AI's Pokémon is slower than the player's and KOs in < hits. Or AI considers Wynaut or Wobbuffet. |
| +1 | AI's Pokémon is faster than the player's. |
| 0 | Default |
| -1 | AI's Pokémon is slower than the player's and is OHKO'd. If Imposter Ditto is considered, this check is skipped. |

If the considered Pokémon is a **Support** and isn’t at -1 Score it gets an *additional +2 score 10% of the time*.

Additionally, the AI checks whether the Pokémon will take damage immediately upon switching in (e.g. from fast Volt Switch or Eject Pack). If so:    
-1: AI's Pokémon is slower and 2HKO’d  
-2: AI's Pokémon is OHKO’d

## Mid-Turn Switch AI

In almost all cases, the AI will only switch if the selected Pokémon has a non-negative switch-in score. If all available candidates have a score below 0, the AI will not switch. Similar to Post-KO Switch AI, each slot is evaluated independently in Double Battles.

Some switch conditions require the *Avoid Switch* check to fail before they can trigger.

Avoid Switch is considered active if any of the following are true:

* The AI has boosted stats  
* The AI can KO one of the player’s Pokémon  
* The player has Pursuit, phazing moves or OHKO moves

Switch decisions are evaluated in priority order.  
Earlier conditions override later ones. 

### Perish Song

* If AI is about to faint to Perish Song  
  * Guaranteed switch

### Palafin

* If AI is Palafin  
* If AI is slower than the player and is OHKO’d  
  * Guaranteed switch

### Anti-Setup AI

* If AI has been in for more than 1 turn  
* If all moves are useless  
  * 40% chance to switch  
  * Random tie-breaking between equal scores

### Anti-Setup AI Plus

* If AI has been active for more than 25 turns  
  * 40% chance to switch  
  * Random tie-breaking between equal scores  
  * Can switch to negative scores 

### Walled AI

* If AI cannot deal meaningful damage ( <= 10% of max HP, increased to 20% if the player has Leftovers, Black Sludge, Leech Seed or Poison Heal active)  
* If AI has been in for more than 5 turns  
* If Avoid Switch fails  
* If it’s a Single Battle  
  * 20% chance to switch

### Support AI

* If AI is a Support  
* If AI has been in for more than 1 turn  
* If Avoid Switch fails  
  * 20% chance to switch

### Weather AI

* If AI has a weather or terrain setting ability (e.g. Drought, Electric Surge)  
* If the corresponding weather or terrain faded  
* If AI has been in for more than 1 turn  
* If Avoid Switch fails  
  * 20% chance to switch

### Anti-Stall AI

* If AI has been in for more than 12 turns  
* If Avoid Switch fails  
  * 20% chance to switch

### Regenerator AI

* If AI has Regenerator  
* If $HP < \frac{maxHP * 2}{3}$  
* If Avoid Switch fails  
  * 40% chance to switch

### Immunity AI

* If AI has an immunity ability that grants an advantage (e.g. Water Absorb, Motor Drive, Wind Rider)  
* If Players last used move type corresponds to that immunity type  
  * 75% chance to switch

## Overview of Switch Conditions

The AI will not switch out without a valid switch-in unless it’s:

* Anti-Setup AI Plus

The AI will send in the Pokemon with the highest Switchin Score, with Team order as a tiebreaker, except for:

* Anti-Setup AI  
* Anti-Setup AI Plus

The Avoid Switch check is used for the following AI’s:

* Walled AI  
* Support AI  
* Weather AI  
* Anti-Stall AI  
* Regenerator AI