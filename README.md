# Rogue C (NCURSES)

A terminal-based dungeon crawler built in C using the `ncurses` library. The game features procedural room generation, floor progression, multiple enemy types, directional combat, inventory management, and an authentication system.

---

## Features

* **Procedural Dungeon Layout**: Randomly sized rooms interconnected with corridors and doorways across multiple floor depths.


* **Combat & Arsenal**: Melee and ranged weapons with varying damage and range values:


* `!` Mace (Melee)


* `%` Sword (Melee)


* `}` Dagger (Ranged)


* `~` Normal Arrow (Ranged)


* `$` Magic Wand (Ranged)




* **Enemies**: Five distinct monster types with different health pools:


* `D` Daemon (5 HP)


* `F` Fire-breathing Monster (10 HP)


* `G` Giant (15 HP)


* `S` Snake (20 HP)


* `U` Undead (30 HP)




* **Loot & Buffs**: Collect gold (`*`), food items (`f`) to restore health, and stat-boosting charms for health (`z`), speed (`x`), and damage (`c`).


* **User Authentication**: Account sign-up, sign-in with password validation, profile inspection, or instant guest access.



---

## Controls

### Movement

Movement follows traditional rogue/vi keys (supports both lowercase and uppercase):

| Key | Direction |
| --- | --- |
| `h` / `l` | Move Left / Right

 |
| `j` / `k` | Move Up / Down

 |
| `y` / `u` | Move Up-Left / Up-Right

 |
| `b` / `n` | Move Down-Left / Down-Right

 |

### Actions & Menus

| Key | Action |
| --- | --- |
| `Space` + (`h`/`j`/`k`/`l`) | Attack in the chosen direction

 |
| `!` / `%` / `}` / `~` / `$` | Equip / Unequip specific weapon

 |
| `i` | Open weapon inventory display

 |
| `e` | Open food menu and consume rations

 |
| `p` | View charm counts

 |
| `>` | Descend through the floor exit

 |
| `q` | Quit current screen or session

 |

---

## Prerequisites

* **GCC** (or any standard C compiler)
* **NCURSES** library headers and development packages

### Installing Dependencies

**Ubuntu / Debian:**

```bash
sudo apt update
sudo apt install build-essential libncurses5-dev libncursesw5-dev

```

**macOS (Homebrew):**

```bash
brew install ncurses

```

---

## Compilation & Run

1. Clone the repository:
```bash
git clone https://github.com/FundamentalOfProgramming-SUT-2024/fop2024-project-sarahzd8.git
cd fop2024-project-sarahzd8

```


2. Compile the source with the `ncurses` link flag:
```bash
gcc Rogue.c -o rogue -lncurses

```


3. Run the executable (make sure your terminal window is at least **136x30** characters for full UI layout):


```bash
./rogue

```
