# Q&A

* **Q: How does AI see multi-hit moves?**  
  **A:** AI usually sees 3 hits for both itself or Player. If the Pokémon has Loaded Dice or Skill Link, it’s 4 hits and 5 hits respectively.

* **Q: How does AI calc Analytic and Payback?**  
  **A:** The AI calculates both Pokémons speed stats and predicts whether Analytic or Payback would apply or not. This does not apply to Avalanche.

* **Q: Does AI understand the Players priority moves?**  
  **A:** No, the AI can only make decisions based on the dynamic speed stats of the Pokémon.

* **Q: What are phazing moves?**  
  **A:** Moves that force the target to switch out: Roar, Whirlwind, Dragon Tail and Circle Throw.

* **Q: Does Switch-in AI factor in hazards, Tailwind, Trick Room, Wonder Room, Magic Room, Mud Sport, Water Sport and 0 PP moves?**  
  **A:** Yes. With the exception of Sticky Web, Switch-in AI takes all of these effects into account when evaluating switch-ins.

* **Q: Does Switch-in AI factor in consumable items such as Electric Seed or Booster Energy?**  
  **A:** No. The AI does not predict item consumption for Pokémon that are not yet on the field. As a result, interactions involving items being consumed on switch-in, particularly with Acrobatics and Unburden, are not considered during switch evaluation.

* **Q: How does Castform on Fisherman Ivan behave? How does AI see transformations that happen when the Pokémon is sent out?**  
  **A:** Generally speaking, Pokémon that haven’t transformed yet will be seen untransformed. Among others, this goes for Wishiwashi, Minior and Castform. Castform has a special case where it would see its Weather Ball damage multiplied by 1.5 to simulate the STAB it would receive.