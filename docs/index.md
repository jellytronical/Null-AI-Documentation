# Pokémon Null AI documentation

![Null AI Logo](assets/logo.png)

This document explains how the AI behaves during a turn. It is not fully exhaustive, and while I have done my best to ensure accuracy, mistakes, omissions, or outdated information may still be present. Most relevant cases are covered, but some moves and score values may be missing. If you notice something important that is incorrect, missing, or unclear, please contact Terra on Discord so it can be reviewed and updated.

The AI assigns a score to every available move and selects the highest-scoring option each turn. If multiple moves share the same score, one is chosen at random. In Double Battles, it evaluates every move against all possible targets and selects the highest-scoring move–target combination. In Null, the AI has full knowledge of your team’s stats, moves, items and abilities from the start of the fight. 

The rest of this document lists the possible move scores and the scenarios in which they apply. As a general rule, **non-attacking moves default to a score of +6** (tied with the highest-damage move: HDM). Exceptions include Nature Power and Memento. Most moves with guaranteed secondary effects (accounting in Serene Grace boosts) and accuracy above 70 (to avoid edge cases like Zap Cannon in Nuzzle AI) also use the +6 base score and follow the behavior of their corresponding status move (e.g. Mystical Fire is treated like Confide). However, these moves do not receive the +6 bonus and do not follow their corresponding AI (unless explicitly stated otherwise) if they are already functioning as the HDM. 

Future Sight also starts with a default score of +6.

The AI also has a basic “useless move” check. For example, it won’t set Stealth Rock if it’s already active, or attempt to inflict a status that is already present. In these cases, the move usually receives a **-20 score penalty**. Not every edge case is listed here, since most are intuitive and including them would add unnecessary bulk. Any non-obvious exceptions will be explicitly noted.

test

