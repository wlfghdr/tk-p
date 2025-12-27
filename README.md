# ⚡️ Timekiller - The Ultimate Reaction Puzzle

<div align="center">

![App Icon](Assets/icon.png)

**Fast-paced puzzle game that tests your reflexes and brain!**

[![Platform](https://img.shields.io/badge/platform-iOS%2017.0%2B-blue.svg)](https://developer.apple.com/ios/)
[![Platform](https://img.shields.io/badge/platform-watchOS-orange.svg)](https://developer.apple.com/watchos/)
[![Swift](https://img.shields.io/badge/Swift-5.9-orange.svg)](https://swift.org)
[![SwiftUI](https://img.shields.io/badge/SwiftUI-5.0-blue.svg)](https://developer.apple.com/xcode/swiftui/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

[English](#english) • [Deutsch](#deutsch)

</div>

---

## English

### 📖 About

Timekiller is an addictive reaction puzzle game where you must identify the correct tile before time runs out! Find the tile where the **text label matches the background** - but watch out, it gets faster with every level!

### ✨ Features

- 🎨 **Three Game Modes**
  - **Colors**: Match color names with backgrounds (8 standard / 16 pro)
  - **Shapes**: Match shape names with symbols (12 standard / 24 pro)
  - **Emojis**: Match emoji names with icons (16 standard / 64 pro)
  
- 📊 **Three Grid Sizes**
  - 2×2: Fast and intense (4 tiles, 8s base time)
  - 2×4: Medium difficulty (8 tiles, 12s base time)
  - 3×5: Maximum challenge (15 tiles, 15s base time)

- 🏆 **Progressive Challenge**
  - Start at Level 1
  - 6 rounds per level
  - Time reduces by 15% each level
  - Exponential score multiplier
  - One mistake = Game Over!

- 🎮 **Advanced Features**
  - 15 unlockable achievements
  - Pro mode with more items (1.5× points)
  - Highscore system (Top 10)
  - Sound & haptic feedback
  - Dark & Light mode
  - Full localization (English & German)
  - Apple Watch companion app

- 🎯 **Scoring System**
  - Base points depend on grid size
  - Multiplied by level (2^(Level-1))
  - Multiplied by time remaining
  - Bonus for shapes (+20%) and emojis (+15%)
  - Pro mode bonus (+50%)


### 🎮 How to Play

1. **Choose Your Mode**: Colors, Shapes, or Emojis
2. **Select Grid Size**: 2×2, 2×4, or 3×5
3. **Tap Start**: The timer begins!
4. **Find the Match**: Tap the tile where text = background
5. **Beat the Clock**: Answer before time runs out
6. **Level Up**: Complete 6 rounds to advance
7. **Go Pro**: Unlock Pro mode for the ultimate challenge!

**One mistake ends the game - stay focused!** ⚡️

### 🏅 Achievement System

Unlock 15 unique achievements by completing challenges:

- **🐻‍❄️ Color Cub**: Complete Level 5 on 2×2 Colors
- **🪢 Rectangle Wrangler**: Complete Level 5 on 2×4 Colors
- **🧙‍♂️ Grid Guru**: Complete Level 5 on 3×5 Colors
- **🧠🎨 Palette Mastermind**: Complete all Color grids → Unlocks Shapes mode
- **🔷 Shape Shifter**: Complete Level 5 on 2×2 Shapes
- **⬡ Polygon Pro**: Complete Level 5 on 2×4 Shapes
- **📐 Geometry Genius**: Complete Level 5 on 3×5 Shapes
- **🏆 Shape Master**: Complete all Shapes grids → Unlocks Emoji mode
- **🙂⬜ Square Smiler**: Complete Level 5 on 2×2 Emojis
- **🚂😄 Emoji Express**: Complete Level 5 on 2×4 Emojis
- **👑😎 Smiley Supreme**: Complete Level 5 on 3×5 Emojis
- **🦸‍♂️✨ Pro Unlocked Hero**: Complete all Emoji grids → Unlocks Pro mode
- **🔥 Pro Mode Masters**: Complete Level 5 on each grid in Pro mode
- **⏳👑 Ultimate Master**: Complete Level 5 on ALL grids in ALL modes

### 💡 Tips & Strategies

- **Focus on the match**, not reading everything
- **Speed is important**, but accuracy matters more!
- Start with **2×2 grid** to learn the mechanics
- **Pro mode** is harder but gives significantly more points
- Use the **time multiplier** to your advantage - answer quickly!
- Each emoji game has **different random emojis** for variety


### 🛠 Technical Details

- **Platform**: iOS 17.0+ / watchOS 10.0+
- **Framework**: SwiftUI
- **Architecture**: MVVM with Observation
- **Storage**: UserDefaults (local persistence)
- **Languages**: English, German

### 📱 Compatibility

- iPhone (iOS 17.0+)
- iPad (optimized)
- Apple Watch (companion app)
- All screen sizes supported
- Dark & Light mode

### 👤 Author

**Wolfgang Heider**
- GitHub: [@wlfghdr](https://github.com/wlfghdr)

### 🎯 Roadmap

- [x] Color mode
- [x] Shape mode  
- [x] Emoji mode
- [x] Achievement system
- [x] Pro mode
- [x] Apple Watch app
- [x] Sound & haptic feedback
- [ ] Additional game modes (numbers, letters)
- [ ] Endless mode
- [ ] Online leaderboards
- [ ] Multiplayer

---

## Deutsch

### 📖 Über die App

Timekiller ist ein süchtig machendes Reaktions-Puzzle, bei dem du die richtige Kachel identifizieren musst, bevor die Zeit abläuft! Finde die Kachel, bei der das **Textlabel mit dem Hintergrund übereinstimmt** - aber Vorsicht, mit jedem Level wird es schneller!

### ✨ Features

- 🎨 **Drei Spielmodi**
  - **Farben**: Farbnamen mit Hintergründen abgleichen (8 Standard / 16 Pro)
  - **Formen**: Formennamen mit Symbolen abgleichen (12 Standard / 24 Pro)
  - **Emojis**: Emoji-Namen mit Icons abgleichen (16 Standard / 64 Pro)
  
- 📊 **Drei Grid-Größen**
  - 2×2: Schnell und intensiv (4 Kacheln, 8s Basis-Zeit)
  - 2×4: Mittlere Schwierigkeit (8 Kacheln, 12s Basis-Zeit)
  - 3×5: Maximale Herausforderung (15 Kacheln, 15s Basis-Zeit)

- 🏆 **Progressive Herausforderung**
  - Start bei Level 1
  - 6 Runden pro Level
  - Zeit reduziert sich um 15% pro Level
  - Exponentieller Score-Multiplikator
  - Ein Fehler = Game Over!

- 🎮 **Erweiterte Features**
  - 15 freischaltbare Errungenschaften
  - Pro-Modus mit mehr Items (1,5× Punkte)
  - Highscore-System (Top 10)
  - Sound & Haptik-Feedback
  - Dark & Light Mode
  - Vollständige Lokalisierung (Deutsch & Englisch)
  - Apple Watch Begleit-App

- 🎯 **Punktesystem**
  - Basispunkte abhängig von Grid-Größe
  - Multipliziert mit Level (2^(Level-1))
  - Multipliziert mit verbleibender Zeit
  - Bonus für Formen (+20%) und Emojis (+15%)
  - Pro-Modus Bonus (+50%)


### 🎮 Spielanleitung

1. **Modus wählen**: Farben, Formen oder Emojis
2. **Grid-Größe auswählen**: 2×2, 2×4 oder 3×5
3. **Start antippen**: Der Timer beginnt!
4. **Match finden**: Tippe die Kachel an, wo Text = Hintergrund
5. **Zeit schlagen**: Antworte bevor die Zeit abläuft
6. **Level aufsteigen**: Schließe 6 Runden ab zum Aufsteigen
7. **Pro werden**: Schalte den Pro-Modus für die ultimative Herausforderung frei!

**Ein Fehler beendet das Spiel - bleib fokussiert!** ⚡️

### 🏅 Errungenschaften-System

Schalte 15 einzigartige Errungenschaften frei, indem du Herausforderungen meisterst:

- **🐻‍❄️ Farb-Bär**: Schließe Level 5 auf 2×2 Farben ab
- **🪢 Rechteck-Ranger**: Schließe Level 5 auf 2×4 Farben ab
- **🧙‍♂️ Grid-Guru**: Schließe Level 5 auf 3×5 Farben ab
- **🧠🎨 Paletten-Meister**: Schließe alle Farben-Grids ab → Schaltet Formen-Modus frei
- **🔷 Formen-Wandler**: Schließe Level 5 auf 2×2 Formen ab
- **⬡ Polygon-Profi**: Schließe Level 5 auf 2×4 Formen ab
- **📐 Geometrie-Genie**: Schließe Level 5 auf 3×5 Formen ab
- **🏆 Formen-Meister**: Schließe alle Formen-Grids ab → Schaltet Emoji-Modus frei
- **🙂⬜ Quadrat-Smiler**: Schließe Level 5 auf 2×2 Emojis ab
- **🚂😄 Emoji-Express**: Schließe Level 5 auf 2×4 Emojis ab
- **👑😎 Smiley-Supreme**: Schließe Level 5 auf 3×5 Emojis ab
- **🦸‍♂️✨ Pro-Freischalt-Held**: Schließe alle Emoji-Grids ab → Schaltet Pro-Modus frei
- **🔥 Pro-Modus-Meister**: Schließe Level 5 auf jedem Grid im Pro-Modus ab
- **⏳👑 Ultimativer Meister**: Schließe Level 5 auf ALLEN Grids in ALLEN Modi ab

### 💡 Tipps & Strategien

- **Konzentriere dich auf die Übereinstimmung**, nicht aufs Lesen von allem
- **Geschwindigkeit ist wichtig**, aber Genauigkeit noch mehr!
- Starte mit dem **2×2 Grid**, um die Mechanik zu lernen
- **Pro-Modus** ist schwieriger, gibt aber deutlich mehr Punkte
- Nutze den **Zeit-Multiplikator** zu deinem Vorteil - antworte schnell!
- Jedes Emoji-Spiel hat **verschiedene zufällige Emojis** für Abwechslung


### 🛠 Technische Details

- **Plattform**: iOS 17.0+ / watchOS 10.0+
- **Framework**: SwiftUI
- **Architektur**: MVVM mit Observation
- **Speicherung**: UserDefaults (lokale Persistenz)
- **Sprachen**: Deutsch, Englisch

### 📱 Kompatibilität

- iPhone (iOS 17.0+)
- iPad (optimiert)
- Apple Watch (Begleit-App)
- Alle Bildschirmgrößen unterstützt
- Dark & Light Mode


### 👤 Autor

**Wolfgang Heider**
- GitHub: [@wlfghdr](https://github.com/wlfghdr)

### 🎯 Roadmap

- [x] Farben-Modus
- [x] Formen-Modus  
- [x] Emoji-Modus
- [x] Errungenschaften-System
- [x] Pro-Modus
- [x] Apple Watch App
- [x] Sound & Haptik-Feedback
- [ ] Zusätzliche Spielmodi (Zahlen, Buchstaben)
- [ ] Endlos-Modus
- [ ] Online-Bestenlisten
- [ ] Multiplayer

---

<div align="center">

⚡️ **How fast can YOU think?** ⚡️

</div>
