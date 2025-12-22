# Timekiller ⚡️

A fast-paced, reaction-based puzzle game for iOS where players race against time to identify the correct tile whose text label matches its background.

![iOS](https://img.shields.io/badge/iOS-17.0%2B-blue)
![Swift](https://img.shields.io/badge/Swift-5.9%2B-orange)
![SwiftUI](https://img.shields.io/badge/SwiftUI-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

## 🎮 Game Overview

**Timekiller** challenges players to quickly identify matching tiles under time pressure. The game features two distinct modes (Colors and Emojis) and progressively increases difficulty through higher levels.

### Game Objective

Find and tap the tile where the **text content matches the background**:
- **Colors Mode**: The text "Blue" must be on a blue tile
- **Emojis Mode**: The text "Ghost" must be next to a 👻 emoji

## ✨ Features

### Game Modes

#### 🎨 Colors Mode
- **Standard**: 8 colors (Red, Blue, Green, Yellow, Orange, Purple, Brown, Cyan)
- **Pro Mode**: 16 colors (+ Gray, Indigo, Mint, Turquoise, Pink, Violet, Beige, Silver)

#### 😀 Emojis Mode
- **Standard**: 16 emojis (randomly mixed each game)
- **Pro Mode**: 64 emojis (randomly mixed each game)

### Grid Sizes
- **2×2**: 4 tiles (faster gameplay, 8s base time)
- **2×4**: 8 tiles (medium, 12s base time)
- **3×4**: 12 tiles (more choices, 15s base time)

### Progressive Difficulty
- Start at configurable levels (1-10)
- Time limit reduces by **12%** per level (factor: 0.88^(Level-1))
- Each level consists of **6 rounds**
- Score multiplier increases exponentially with level

### Scoring System

**Base Points** (per round):
- 2×2 Grid: 10 points
- 2×4 Grid: 14 points
- 3×4 Grid: 18 points

**Multipliers**:
- **Level Multiplier**: 2^(Level-1)
- **Emoji Bonus**: 1.3× (30% more points)
- **Pro Mode Bonus**: 1.5× (50% more points)

**Formula**:
```
Final Score = Base Points × Level Multiplier × Emoji Bonus × Pro Bonus
```

**Point Awards**:
- ✅ Correct Answer: + Calculated points
- ❌ Wrong Answer: - Calculated points
- ⏱️ Timeout: 0 points

### Game Over Conditions
1. Level score is negative or zero after 6 rounds
2. 2 consecutive wrong answers
3. 2 consecutive timeouts
4. Player chooses "Quit"

## 📱 User Interface

### Main Game Screen
- **Header**: Level, round progress, scores, timer, grid info
- **Game Grid**: Dynamic tile layout based on settings
- **Progress Bar**: Visual time indicator (green/red)
- **Score Overlay**: Animated score feedback after each answer

### Additional Screens
- **Start Screen**: Mode selection, example grid, instructions
- **Pause Screen**: Resume or quit options
- **Level Complete**: Celebration screen with continue/quit options
- **Summary Screen**: Game over stats, score breakdown, top 3 preview
- **Settings**: Comprehensive game configuration
- **Highscores**: Top 10 scores with swipe-to-delete

## 🛠 Technical Details

### Requirements
- **Platform**: iOS 17.0+
- **Language**: Swift 5.9+
- **Framework**: SwiftUI
- **State Management**: Observation Framework (`@Observable`)
- **Persistence**: UserDefaults with JSON encoding

### Architecture
- Pure SwiftUI implementation
- Modern Swift concurrency patterns
- Reactive state management
- Localized for German and English

### Key Technologies
- **SwiftUI**: Complete UI implementation
- **Observation Framework**: Modern state management
- **Foundation**: Core functionality
- **UserDefaults**: Data persistence

## 🌍 Localization

Timekiller supports multiple languages:
- 🇩🇪 German (Deutsch)
- 🇬🇧 English

The app automatically detects the system language and uses German if available, otherwise defaults to English. All UI text, color names, and emoji descriptions are fully localized.

## 🎯 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/timekiller.git
```

2. Open the project in Xcode 15 or later:
```bash
cd timekiller
open Timekiller.xcodeproj
```

3. Build and run on your device or simulator (iOS 17.0+)

## 🎮 How to Play

1. **Choose Your Mode**: Select Colors or Emojis
2. **Pick Grid Size**: Choose from 2×2, 2×4, or 3×4
3. **Optional**: Enable Pro Mode for extra challenge
4. **Start Playing**: Tap the correct tile before time runs out
5. **Progress**: Complete 6 rounds to advance to the next level
6. **Compete**: Beat your high score and climb the leaderboard

### Tips
- 💡 Focus on finding the match, not reading everything
- ⚡️ Speed matters, but accuracy matters more (wrong answers deduct points!)
- 🎯 Start with 2×2 grid to learn the mechanics
- 🏆 Pro Mode doubles the difficulty but also doubles the rewards

## 📊 Settings

Customize your experience:
- **Game Mode**: Colors or Emojis
- **Grid Size**: 2×2, 2×4, or 3×4
- **Difficulty**: Pro Mode toggle
- **Start Level**: Begin at levels 1-10
- **Player Name**: Personalize your highscore entries
- **Theme**: System, Light, or Dark
- **Language**: German or English

## 🏆 Highscores

- **Top 10**: Only the best 10 scores are saved
- **Persistent**: Scores are saved between sessions
- **Details**: View player name, score, max level, and date
- **Management**: Swipe to delete entries

## 🧪 Testing

The project includes:
- **Unit Tests**: Score calculation, level progression, timer functionality
- **UI Tests**: Navigation, button responses, settings persistence
- **Manual Tests**: Cross-device compatibility, performance, accessibility

## 🚀 Future Enhancements

Potential features for future versions:
- 🎵 Sound effects and haptic feedback
- 🏅 Achievement system
- 📊 Detailed statistics and analytics
- 🌐 Global leaderboards
- 🎨 Custom color themes
- 🎓 Tutorial mode
- ♾️ Endless mode
- 👥 Multiplayer battles

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**Wolfgang Heider**

## 🙏 Acknowledgments

- Built with SwiftUI and modern Swift features
- Designed for iPhone and iPad
- Optimized for iOS 17.0+

---

**Version**: 1.0  
**Date**: December 22, 2024  

Enjoy playing Timekiller! ⚡️🎮
