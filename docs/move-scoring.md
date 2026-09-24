<a id="move-scoring"></a>
# Move scoring

The AI assigns a score to every available move and selects the highest-scoring option each turn. If multiple moves share the same score, one is chosen at random. In Double Battles, it evaluates every move against all possible targets and selects the highest-scoring move–target combination. In Null, the AI has full knowledge of your team’s stats, moves, items and abilities from the start of the fight. 

The rest of this document lists the possible move scores and the scenarios in which they apply. As a general rule, **non-attacking moves default to a score of +6**, tied with the highest-damage move (HDM). Exceptions include Nature Power and Memento. Most moves with guaranteed secondary effects (accounting for Serene Grace boosts) and accuracy above 70 (to avoid edge cases like Zap Cannon in Nuzzle AI) also use the +6 base score and follow the behavior of their corresponding status move (e.g. Mystical Fire is treated like Confide). However, these moves do not receive the +6 bonus and do not follow their corresponding AI (unless explicitly stated otherwise) if they are already functioning as the HDM. Future Sight also starts with a default score of +6.

The AI also has a basic “useless move” check. For example, it won’t set Stealth Rock if it’s already active, or attempt to inflict a status that is already present. In these cases, the move usually receives a **-20 score penalty**. Not every edge case is listed here, since most are intuitive and including them would add unnecessary bulk. Any non-obvious exceptions will be explicitly noted.

<a id="common-scores"></a>
## Common scores

| Move | Probability |
| --- | --- |
| **Highest damaging move (HDM)** | +6 (75%), +8 (25%) |
| **Slow kill** (AI kills but is slower than target) | +9 (75%), +11 (25%) |
| **Fast kill** (AI kills and is faster* than target) | +12 (75%), +14 (25%) |

*AI sees speed ties as being faster than the player and priority move kill counts as a fast kill.

<a id="damaging-moves"></a>
## Damaging moves

AI will roll a random damage value for all of its attacking moves, and the highest damaging move (HDM) gets the following score: +6 (75%), +8 (25%)  
If multiple moves kill, then they are all considered HDM and all get this score.  
There are a few specific damaging moves that do not have their damage rolled normally and are thus never considered HDM. These moves are:

* Explosion, Self-Destruct, Misty Explosion  
* Final Gambit  
* Meteor Beam   
* Future Sight  
* OHKO moves  
* Feint, Upper Hand

<a id="if-a-damaging-move-kills"></a>
### If a damaging move kills

* If AI is faster or the move has priority and AI is slower: +6 Score  
* If AI is slower: +3 Score  
  * The following moves do not receive a kill bonus: Explosion, Self-Destruct, Misty Explosion, Final Gambit, Rollout, Ice Ball, OHKO moves  
  * The following moves receive a kill bonus, despite never being considered as HDM: Meteor Beam, Future Sight.  
* If AI has Moxie, Beast Boost, Chilling Neigh, or Grim Neigh: +1 Score

<a id="damaging-priority-moves-feint-excluded"></a>
### Damaging priority moves (Feint excluded)

* If AI is slower and Player can faint AI:  
  * If the priority move is also HDM: +5 Score  
  * Else: +11 Score  
* Else if AI is slower and has Eject Button: +11 Score

<a id="score-priority-overview"></a>
## Score priority overview

The following provides a high-level overview of how maximum move scores are prioritized within the AI logic. This list is not exhaustive and is only intended to illustrate the general hierarchy and relative score priority of different decision outcomes.

<a id="tier-1"></a>
### Tier 1
* Fast kill  
* Palafin Flip Turn  
* If frozen: Moves that thaw the user  
* Damaging Gimmick moves (Feint, Upper Hand, Beat Up, Round, Weakness Policy activation, Pursuit, if user has a negative ability and target has a Mummy-like ability)  
* Protect (For achieving form change gimmicks, e.g Power Construct, Stance Change, Zen Mode)  

<a id="tier-2"></a>
### Tier 2
* Slow kill  
* Field moves:   
    * Trick Room, Wonder Room, Magic Room, Gravity, Mud Sport, Water Sport  
    * Hazards, Tailwind  
* With Power Herb: 2-turn moves with powerful side effects (Geomancy, Meteor Beam, Electro Shot, Sky Attack, Freeze Shock, Ice Burn)  
* Boosting a partners stats  
    * Swagger and Flatter if the partner will not be confused  
    * Coaching, Decorate  
* Status Gimmick moves (Psych Up, Role Play, etc)  

<a id="tier-3"></a>
### Tier 3
* Highest Damage move (HDM)  
* Status moves  
* Damaging moves with guaranteed side-effects (doesn’t stack with HDM score)

<a id="choice-ai"></a>
## Choice AI
If AI is holding a Choice Item: -20 Score to all status moves except:

Memento, Parting Shot, Baton Pass, Teleport, Chilly Reception, Sleep Talk, Me First, Copycat, Mimic, Transform, Sketch, Nature Power, Assist, Metronome.

<a id="should-ai-recover-function"></a>
## Should AI Recover function  

* **Recovery %:**  
    * Standard recovery moves (Recover, Slack Off, Heal Order, Roost, Strength Sap): 50%  
    * Weather-based recovery moves (Morning Sun, Synthesis, Moonlight): 67%  
    * Rest: 100%

* If AI mon is Toxic'd and move isn’t Rest:  
    * Returns False  
* If player mon does as much or more damage than would be healed off:  
    * Returns False  
    * *Note that this calculation uses the Recovery % listed above.*

* If AI is faster:  
    * If player mon can kill AI mon, but cannot after AI mon uses recovery move:  
        * Returns True  
    * If player mon cannot kill AI mon:  
        * If AI mon is below 66% and above 40%:  
            * Returns True (50%), Returns False (50%)  
        * If AI mon is below 40%:  
            * Returns True

* If AI is slower:  
    * If AI is below 70% HP:  
        * Returns True (75%), Returns False (25%)  
    * If AI is below 50% HP:  
        * Returns True  
          
* If none of the above cases are true, then this function defaults to return False.