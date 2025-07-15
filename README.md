# Dragon Repeller RPG

A simple text-based RPG game where you must defeat the dragon that is preventing people from leaving the town. Built with HTML, CSS, and JavaScript.

## 🎮 Game Overview

Dragon Repeller is a browser-based role-playing game where players navigate through different locations, fight monsters, buy equipment, and ultimately face the dragon to win the game.

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No additional software required

### Installation
1. Download or clone the game files
2. Ensure all three files are in the same directory:
   - `gioco.html` (main HTML file)
   - `giocoJavaScript.js` (game logic)
   - `giocoStyles.css` (styling)
3. Open `gioco.html` in your web browser to start playing

## 🎯 How to Play

### Starting Stats
- **Health**: 100
- **Gold**: 50
- **XP**: 0
- **Starting Weapon**: Stick (power: 5)

### Game Locations

#### Town Square
Your starting location with three options:
- **Go to Store**: Purchase health and weapons
- **Go to Cave**: Fight monsters to gain XP and gold
- **Fight Dragon**: The ultimate challenge (not recommended early game!)

#### Store
- **Buy Health**: 10 gold for 10 health points
- **Buy Weapon**: 30 gold for the next weapon tier
- **Sell Weapon**: 15 gold (only when you have the most powerful weapon)

#### Cave
Fight monsters to gain experience and gold:
- **Slime**: Level 2, 15 health
- **Fanged Beast**: Level 8, 60 health

### Combat System
- **Attack**: Deal damage based on your weapon + XP bonus
- **Dodge**: Avoid the monster's attack
- **Run**: Escape back to town square

### Weapons Progression
1. **Stick** (power: 5) - Starting weapon
2. **Dagger** (power: 30) - 30 gold
3. **Claw Hammer** (power: 50) - 30 gold
4. **Sword** (power: 100) - 30 gold

### Win Conditions
- Defeat the dragon to win the game
- The dragon has 300 health and is level 20

### Easter Egg
Hidden mini-game accessible after defeating monsters - try clicking the third button multiple times after winning a fight!

## 🛠️ Game Features

- **Dynamic Combat**: Damage calculations include weapon power, XP bonuses, and random elements
- **Weapon Durability**: 10% chance weapons break during combat
- **Progressive Difficulty**: Monsters get stronger as you progress
- **Inventory Management**: Track your weapons and items
- **Hidden Content**: Secret mini-game for extra rewards

## 📁 File Structure

```
dragon-repeller/
├── gioco.html           # Main game HTML structure
├── giocoJavaScript.js   # Game logic and mechanics
└── giocoStyles.css      # Visual styling
```

## 🎨 Technical Details

### Technologies Used
- **HTML5**: Game structure and layout
- **CSS3**: Styling and visual design
- **Vanilla JavaScript**: Game logic and interactivity

### Key JavaScript Features
- Object-oriented design with location and monster data structures
- Dynamic UI updates based on game state
- Event-driven gameplay with button interactions
- Random number generation for combat and mini-games

## 🎲 Game Mechanics

### Combat Formula
- **Player Attack**: `weapon_power + random(0, xp) + 1`
- **Monster Attack**: `(monster_level * 5) - random(0, xp)`
- **Hit Chance**: 80% base chance (100% if health < 20)

### Rewards
- **Gold**: `monster_level * 6.7` (rounded down)
- **Experience**: `monster_level` points per defeated monster

## 🐛 Known Issues & Tips

- Save your progress by keeping the browser tab open
- Don't sell your only weapon!
- Build up XP fighting weaker monsters before challenging the dragon
- Higher XP reduces incoming damage and increases your attack power

## 📝 License

This project is open source and available under standard educational use.

**Enjoy your adventure in Dragon GAME!** 🐉⚔️
