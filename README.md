# Untitled RPG

A hunting RPG where you move with the left and right arrow keys, attack with Z and X and reload with space. Money from hunting buys shields, and there is even a skill merchant to trade with.

<p>
  <img src="docs/screenshots/screenshot-1.png" width="216" alt="Gameplay">
</p>


## How to play

Download from Releases and run it.

Move with the left and right arrow keys, and click the on screen buttons to go up or down. Attack with Z and X, and reload with space. Killing enemies in the hunting grounds earns money, and shields and skills can be bought in the village.


## How it works

The attack cooldown is built from object collisions instead of an alarm. Attacking changes the character into a cooldown state object, and reloading with space sends two objects off toward each other at speed 1. The moment they meet and trigger a collision event is when the cooldown ends, at which point they change the character back into the ready to attack object and delete themselves. How far apart the two objects start is the cooldown time. The shield cooldown works the same way with another pair of objects, and pressing the attack key during a cooldown shows a notice.


## Files

| Path | Contents |
|---|---|
| `source/untitled-rpg.gmk` | Original project file |
| `source/split/` | Text tree produced by GmkSplitter |
| `docs/screenshots/` | Screenshots |
| Releases | Distributed build |


## License

CC BY-NC-ND 4.0. Unmodified copies may be shared for noncommercial purposes with attribution. Modified versions and commercial use are not allowed. Bundled libraries, graphics, sounds, and maps made by other people keep their own rights. See [LICENSE](LICENSE).
