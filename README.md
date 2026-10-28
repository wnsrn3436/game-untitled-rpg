# Untitled RPG

[한국어](README.ko.md)

A hunting RPG where you move with the left and right arrow keys, attack with Z and X, and reload with space. You can even spend the money you collect from hunting on shields and trade with a skill merchant.

<p>
  <img src="docs/screenshots/screenshot-1.png" width="216" alt="Gameplay">
</p>


## How to play

Download it from Releases and run it.

Move with the left and right arrow keys, and click the on-screen buttons to go up or down. Attack with Z and X, and reload with space. Killing enemies in the hunting grounds earns money, and you can buy shields and skills in the village.


## How it works

The attack cooldown is built from object collisions instead of an alarm. Attacking turns the character into a cooldown-state object, and reloading with space sends two objects off toward each other at speed 1. The cooldown ends the moment they meet and trigger a collision event. At that point they turn the character back into the object that can attack and delete themselves. The distance you place between the two objects becomes the cooldown time. The shield cooldown works the same way with another pair of objects, and pressing the attack key during a cooldown shows a notice.


## Files

| Path | Contents |
|---|---|
| `source/untitled-rpg.gmk` | Original project file |
| `source/split/` | Text tree produced by GmkSplitter |
| `docs/screenshots/` | Screenshots |
| Releases | Distributed build |


## License

CC BY-NC-ND 4.0. Unmodified copies may be shared for noncommercial purposes with attribution. Distributing modified versions and commercial use are not allowed. Bundled libraries, graphics, sounds, and maps made by other people keep their own rights. See [LICENSE](LICENSE).
