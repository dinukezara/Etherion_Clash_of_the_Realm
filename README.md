# 🎮 Etherion: Clash of Realms

**Etherion: Clash of Realms** is a turn-based RPG developed in **Java**. The game combines elemental combat, strategic power selection, character upgrades, and player progression across mystical realms.

## 🧩 Game Overview

Players begin their journey by choosing an elemental affinity and building their character for battle.

- 🔥 Choose an elemental affinity: **Fire, Water, Earth, or Air**
- ⚔️ Battle unique villains across **12 missions**
- 🧙 Use special powers during combat
- 🛡️ Equip shields to improve your defense
- 🛒 Earn coins and purchase characters, powers, and shields
- 📈 Level up and unlock increasingly difficult challenges

## 🏗️ Features

- Turn-based combat system
- Dynamic damage calculation
- Object-Oriented Programming (OOP) design
- Multiple hero and villain characters
- Elemental affinity system
- Powers and shields
- Player inventory and progression
- In-game shop system
- 12 mission-based battles
- CSV-based game data
- Save and load functionality using Java Serialization
- CLI-based menus for battles, shop, and player profile

## 🗂️ Project Structure

```text
Etherion_Clash_of_Realms/
│
├── data/
│   ├── Data_Heros.csv
│   ├── Data_Villians.csv
│   ├── Data_Mission.csv
│   ├── Data_Powers.csv
│   └── Data_Shields.csv
│
├── src/
│   ├── Main.java
│   ├── GameEngine.java
│   ├── Battle.java
│   ├── Player.java
│   ├── Character.java
│   ├── HeroChar.java
│   ├── Villain.java
│   ├── Power.java
│   ├── Shield.java
│   └── GameDataLoader.java
│
└── README.md
```

### Main Classes

| Class | Description |
|---|---|
| `Main.java` | Entry point of the game |
| `GameEngine.java` | Handles menus, player creation, and the main game loop |
| `Battle.java` | Contains the battle system logic |
| `Player.java` | Stores player information, inventory, level, and stats |
| `Character.java` | Abstract base class for game characters |
| `HeroChar.java` | Represents player-controlled heroes |
| `Villain.java` | Represents enemies encountered during missions |
| `Power.java` | Represents combat powers and their attack values |
| `Shield.java` | Represents shields and defensive bonuses |
| `GameDataLoader.java` | Loads game information from CSV files |

## 🚀 Getting Started

### Prerequisites

Make sure you have:

- **Java JDK 17 or higher**
- A terminal or Java-compatible IDE such as IntelliJ IDEA, Eclipse, or VS Code

Check your Java installation:

```bash
java -version
javac -version
```

## ▶️ Running the Game

Clone the repository:

```bash
git clone https://github.com/dinukezara/Etherion_Clash_of_the_Realm.git
```

Navigate into the project:

```bash
cd Etherion_Clash_of_the_Realm
```

Compile the Java source files:

```bash
javac src/*.java
```

Run the game:

```bash
java src/Main
```

> Depending on the package declarations used in the Java files, the run command may need to be adjusted.

## ⚔️ Combat System

Battles are turn-based and use character statistics, powers, shields, and speed to calculate damage.

### Damage Formula

```text
Damage =
(AttackerAttack × PowerAttack × (1 + AttackerSpeed))
-----------------------------------------------------
(OpponentDefense + ShieldDefense + 10 × (1 - OpponentSpeed))
```

### Battle Rules

- Characters begin battles with full HP.
- Players select powers to attack opponents.
- Shields increase defensive capability.
- Combat continues until either the player or opponent reaches `0 HP`.
- Winning battles rewards progression and coins.
- Losing a battle results in a penalty.

## 🛒 Shop System

Coins earned during gameplay can be used in the shop.

Players can:

- ⚡ Purchase new powers
- 🎯 Equip up to **4 powers**
- 🛡️ Purchase and unlock shields
- 🧙 Upgrade to stronger hero characters
- 🔓 Unlock items as their level increases

## 💾 Save & Load System

Game progress can be stored using **Java Serialization**.

The saved game contains information such as:

- Player details
- Current level
- Inventory
- Purchased items
- Player progression

The game state is stored in:

```text
savegame.dat
```

Use the following options from the main menu:

```text
Save Game → Save current progress
Load Game → Continue from a previous save
```

## 📊 Game Data

Game information is stored in CSV files inside the `data/` directory.

```text
Data_Heros.csv
Data_Villians.csv
Data_Mission.csv
Data_Powers.csv
Data_Shields.csv
```

These files are loaded into the game through:

```text
GameDataLoader.java
```

This approach separates game data from the main Java source code and makes the game's content easier to maintain.

## 🛠️ Technologies & Tools

- ☕ Java 17
- 📄 CSV
- 💾 Java Serialization
- 🔀 Git
- 🐙 GitHub
- 🎨 Canva
- 📐 Diagrams.net

## 👤 Original Project Owner

**Lakmana Thabrew**

## 🤝 Contributors

This repository may contain work from multiple contributors.

Please refer to the GitHub repository's contributor history for individual contributions.

## 📜 License & Usage

This project was created for **academic and personal development purposes**.

Please contact the project owner and relevant contributors before reusing, redistributing, or modifying their work.

---

⭐ **Etherion: Clash of Realms** — Battle, upgrade, and conquer the realms.
