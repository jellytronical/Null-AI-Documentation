# Damage Move Usability Checks

Normally, the AI prefers the move with the highest damage, referred to as the Highest Damage Move (HDM). However, some moves are unusable under specific conditions. If the AI simply selected the HDM and applied a score penalty afterward, it could end up choosing a random damaging move instead of the second strongest option. To prevent this, the AI checks whether a move is usable before comparing its damage. If a move is considered unusable, its calculated damage is set to 0, allowing the AI to correctly identify the next highest damage option. **This check works in both directions**. The AI uses it when deciding which moves to use itself, but also when calculating the damage of moves the player might use.

The following is a complete breakdown of the conditions covered by this check:

| Move or move category | Unusable condition |
| --- | --- |
| **Sound Moves** | AI is under **Throat Chop Timer** |
| **Healing Moves** | AI has **Heal Block Status** |
| **A Commander pokemon (Tatsugiri)** | **Commanding Dondozo** (It’s unable to make damages but could be targeted in that state) |
| **Electric-Type Moves** | Player has **Volt Absorb** / **Motor Drive** / **Lightning Rod** |
| **Water-Type Moves** | Player has **Water Absorb** / **Dry Skin** / **Storm Draiin** |
| **Fire-Type Moves** | Player has **Flash Fire** |
| **Grass-Type Moves** | Player has **Sap Sipper** |
| **Ground-Type Moves** | Player has **Earth Eater** |
| **Sound Moves** | Player has **Soundproof** |
| **Ballistic Moves** | Player has **Bulletproof** |
| **Wind Moves** | Player has **Wind Rider** |
| **Priority Moves** | Player has **Dazzling** / **Armor Tail** / **Queenly Majesty** |
| **Dream Eater** | Player **isn’t Asleep** / has **Comatose** |
| **Gigaton Hammer** | AI **used it Last Turn** |
| **Belch** | AI didn’t **use a Berry yet** |
| **Last Resort** | AI didn’t use **All of its Other Moves Yet** |
| **Attack that Removes Terrain** | There’s **No Terrain** |
| **Poltergeist** | Player **isn’t Holding an Item** |
| **Burn Up** | AI **isn’t Fire-Type** |
| **Future Sight** | Player **is already under Future Sight** |
| **Sucker Punch / Thunder Clap** | The **Last Move is Sucker Punch / Thunder Clap** **(66.6%)** |
| **Meteor Beam** | AI **isn’t Holding / can’t use Power Herb** |
| **Electro Shot** | AI **isn’t Holding / can’t use Power Herb and it’s not Raining** |
| **Freeze Shock / Sky Attack / Ice Burn** | AI **isn’t Holding / can’t use Power Herb** |
| **Fake Out** | It’s not AI’s **First Turn Out** |
