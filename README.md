# Star Wars: The Force Unleashed – Split-Screen Co-op Mod (PC)

> ## GOG or Steam? Use the GOG version if you can
>
> The mod works on both the **GOG** and the **Steam** release of *Ultimate Sith Edition*. The game code is identical in both, but they get different amounts of memory:
>
> | | GOG | Steam |
> |---|---|---|
> | Memory the game can use | **4 GB** (INSTALL.bat applies the 4 GB patch) | **2 GB** (the patch can't be applied) |
> | Big levels with lots of spawned characters | Plenty of room | Gets tight sooner |
> | Players far apart in a level | Plenty of room | Gets tight sooner |
>
> **Why Steam is limited to 2 GB:** the game is a 32-bit program, so by default Windows gives it only 2 GB of memory. The 4 GB patch changes one setting in `SWTFU.exe` so Windows gives it 4 GB. The Steam `SWTFU.exe` is protected by Steam's copy protection, which refuses to start a changed exe (you'd get *"Application load error 3:0000065432"*). So INSTALL.bat leaves the Steam exe alone, and the game runs with 2 GB.
>
> **Why 4 GB is worth having:** co-op keeps two players' areas of the level active at once, and every character you spawn from the mod menu (troopers, Rancors, bosses ...) loads more models into memory. With 4 GB there is room to spare for all of that. With 2 GB the game runs low sooner. The mod watches free memory and pulls Player 2 back next to Player 1 before it runs out, so it won't crash, but the players can't spread out as far or spawn as much.
>
> **What to do on Steam:** normal co-op play works fine. Go easy on spawning many big characters at once. If Steam ever "verifies" or updates the game, just run INSTALL.bat again.
>
> If you own both versions, play the GOG one.

> **Made for controllers.** Both players play with a gamepad. PC (mouse and keyboard) controls for Player 2 are **not implemented yet**.
>
> **You need your own copy of the game.** This mod contains no game files. It works with the **GOG** (v1.2) and **Steam** releases of *Star Wars: The Force Unleashed – Ultimate Sith Edition* (see above for why GOG is the better choice). At every start the mod checks that your `SWTFU.exe` contains the game code it was built for. On any other version it switches itself off and the game runs normally.
>
> **PlayStation controllers work.** The mod reads Xbox-style (XInput) pads, so a DualShock 4 / DualSense needs Steam Input or DS4Windows. See [Controllers](#controllers).

Two players play the whole story campaign together on one PC, each with their own half of the screen and their own camera. Built for the GOG release (Ultimate Sith Edition, v1.2), also runs on the Steam release, and tested on a ROG Ally connected to a TV.

**Download:** get the newest zip from the [Releases page](../../releases/latest).

---

## Mod menu

**Open or close it with RB + D-pad Up**, on either controller. Each player gets his own menu in his own half of the screen. While a player's menu is open, his character stands still.

| Button | What it does |
|---|---|
| D-pad Up / Down | Move through the list |
| D-pad Left / Right | Change page, or switch an ON/OFF item |
| A | Use the selected item |
| B | Back / close |

| Menu item | What it does |
|---|---|
| GOD MODE PLAYER 1 / PLAYER 2 | That player can't be hurt |
| INFINITE FORCE P1 / P2 | That player's Force bar never runs out |
| TELEPORT ME TO PLAYER x | Moves you next to the other player (useful for elevators and one-player doors) |
| BRING PLAYER x TO ME | Moves the other player next to you |
| SPAWN FRIEND > | Spawns a character that fights **on your side** (troopers, rebels, creatures, droids, bosses) |
| SPAWN ENEMY > | Spawns a character that fights **against you** |
| MY COSTUME > | Changes **your** costume only (each player can wear a different one) |
| NEAREST ENEMY -> FRIEND | Makes the closest enemy fight for you |
| ALL NEAR ENEMIES -> FRIENDS | Makes every nearby enemy fight for you |
| FRIENDLY FIRE: ON/OFF | **Off by default.** When off, the players can't hurt or Force-grab each other |
| UNLOCK EVERYTHING: ON/OFF | All Force powers, upgrades, combos, talents, costumes and crystals for both players. Made to keep saving normally |
| FULL HEALTH (BOTH) | Refills both players |
| REMOVE SPAWNED | Removes everything you spawned |
| CLOSE | Closes the menu |

Spawning notes:
- Characters from other levels are loaded on demand. If one can't be loaded in the current level, the menu says **NOT LOADABLE YET** instead of crashing.
- Big creatures (Rancors, Wampa, Junk Titan) can be spawned in any level with enough room; in tight spaces they refuse and say **TOO BIG TO FIT HERE**.
- Spawned bosses fight with their own lightsaber combos and Force powers. They never start their story finisher cutscenes; those are kept for the real story fights.

## Other button combos

| Combo | What it does |
|---|---|
| Both players hold **BACK** for 2 seconds | Swap Player 1 and Player 2 controllers |
| Player 1 holds **BACK + START** for 3 seconds (or keyboard **F7**) | Emergency: switch co-op off (back to normal single player) and on again |
| **START** on either controller | Pause |
| Keyboard **F8** | Switch between vertical (default) and horizontal split |

## Features

- **Split screen for the whole campaign.** Vertical by default (horizontal with F8). Each half shows its own player's camera.
- **Each player has his own HUD.** You get the game's own health and Force bars, and the target box shows what your Force powers will grab.
- **Cutscenes play full screen.** Short in-game moments stay split. Interactive boss moments (button prompts) go full screen for the player doing them when only the boss is left. If other enemies are still around, the split stays so the other player can keep fighting.
- **Co-op death rule.** A player whose health runs out is *downed*: his half goes dark for 10 seconds, then he comes back next to the other player with full health. If both players go down, the game restarts from the checkpoint.
- **Plug-and-play controllers.** Players follow the controllers that are connected, not fixed slots. A ROG Ally turning off its built-in controller when a Bluetooth pad connects does not mix up who is Player 1.
- **1080p full screen**, widescreen, on a TV or the handheld screen.
- **Large Address Aware (4 GB) patch** for SWTFU.exe so spawns from other levels fit in memory (a backup of the original exe is kept; GOG only).
- **Each half draws its own player's surroundings**, so the two views never mix: no flicker, no giant pieces of the level floating into the picture.

## Controllers

The mod uses **XInput** (Xbox-style) controllers:

- **Xbox controllers** (wired or Bluetooth), the **ROG Ally's built-in controls**, and other XInput pads work directly.
- **PlayStation DualShock 4 / DualSense**: Windows does not show these as XInput by itself. Use one of these:
  1. **Steam Input** (easiest): add `SWTFU.exe` to Steam as a *non-Steam game*, start it from Steam, and enable PlayStation Configuration Support in Steam's controller settings.
  2. **DS4Windows** (free): run it before starting the game. It makes the PlayStation pad look like an Xbox controller.

  Button names in this README use Xbox labels: **A = Cross, B = Circle, X = Square, Y = Triangle, RB = R1, LB = L1, BACK = Share/Create, START = Options.**

## Installing

1. Own and install *Star Wars: The Force Unleashed – Ultimate Sith Edition*: the GOG version (v1.2, recommended) or the Steam version.
2. Extract the contents of the zip **into your game folder** (the folder that contains `SWTFU.exe`; on Steam: right-click the game - Manage - Browse local files). You should then have `dinput8.dll`, `INSTALL.bat` and the `coop` and `tools` folders next to `SWTFU.exe`.
3. Double-click `INSTALL.bat` once. It:
   - applies the 4 GB memory patch to `SWTFU.exe` (a backup is kept as `SWTFU.exe.before_4gb`; skipped on Steam, see above),
   - switches the game to controller mode,
   - sets full screen at 1080p (or the screen's size if it is smaller).

   If it says the game config folder was not found, start the game once, quit, and run `INSTALL.bat` again.
4. Connect two controllers and start the game as usual.

**Updating from an older version:** extract the new zip over the old files (say yes to replace) and run `INSTALL.bat` again.

**Uninstall:** run `UNINSTALL.bat` (deletes `dinput8.dll` and puts the original `SWTFU.exe` back). Your saves are not touched.

## Logs and troubleshooting

- The mod writes `coop\coop_log.txt`. Older logs are kept in `coop\old_logs` and are never deleted. Please attach the log when you report a problem.
- **Game frozen:** run `CLOSE_GAME.bat`.

## Known limitations

- Player 2 can't use mouse and keyboard yet.
- When a player uses Force Push, a faint see-through trace of the other player's view can show in his half for a moment.
- When the players are far apart, a lightsaber can drift out of its player's hand; it snaps back once you get closer again.
- Clone Trooper as a spawnable AI enemy/friend is not available yet. The PC game only has the clone trooper as a player costume, which you can still pick in MY COSTUME.

## Version history

- **v1.1** (19 Nov 2026): split-screen drawing fixed (no flicker, no giant black walls or floating pieces of the level, players and walls no longer vanish), Steam support, screens above 1080p (e.g. a 4K TV) switched to the game's size while it runs, saber and Player 2 fixes.
- **v1.0** (11 Nov 2026): first release.

## Credits

Made for playing the campaign with my son. Star Wars: The Force Unleashed is © Lucasfilm Ltd. / LucasArts; PC version by Aspyr. This is an unofficial fan mod, not affiliated with or endorsed by them.
