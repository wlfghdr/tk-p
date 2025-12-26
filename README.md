# Timekiller ⚡️

Docs index: [assistant-notes.md](assistant-notes.md) · [CLAUDE.md](CLAUDE.md) · [REQUIREMENTS.md](REQUIREMENTS.md)

A fast-paced, reaction-based puzzle game for iOS where players race against time to identify the correct tile whose text label matches its background.

![iOS](https://img.shields.io/badge/iOS-17.0%2B-blue)
![Swift](https://img.shields.io/badge/Swift-5.9%2B-orange)
![SwiftUI](https://img.shields.io/badge/SwiftUI-green)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

## 🎮 Game Overview

**Timekiller** challenges players to quickly identify matching tiles under time pressure. The game features three distinct modes (Colors, Shapes, and Emojis) and progressively increases difficulty through higher levels.

### Game Objective

Find and tap the tile where the **text content matches the background**:
- **Colors Mode**: The text "Blue" must be on a blue tile
- **Shapes Mode**: The text "Circle" must be next to a ● shape
- **Emojis Mode**: The text "Ghost" must be next to a 👻 emoji

## ✨ Features

### Game Modes

#### 🎨 Colors Mode
- **Standard**: 8 colors (Red, Blue, Green, Yellow, Orange, Purple, Brown, Cyan)
- **Pro Mode**: 16 colors (+ Gray, Indigo, Mint, Turquoise, Pink, Violet, Beige, Silver)

#### 🔷 Shapes Mode
- **Standard**: 12 shapes (Circle, Square, Triangle, Star, Diamond, Heart, Hexagon, and more)
- **Pro Mode**: 24 shapes (more variety and challenge)

#### 😀 Emojis Mode
- **Standard**: 16 emojis (randomly mixed each game)
- **Pro Mode**: 64 emojis (randomly mixed each game)

### Sound & Haptic Feedback 🔊

Experience immersive gameplay with sound effects and haptic feedback:
- **Correct Answer**: Success haptic + satisfying sound
- **Wrong Answer**: Error haptic + negative feedback sound
- **Time Warning**: Alert haptic when time is running low (< 25%)
- **Timeout**: Timeout haptic + sound effect
- **Level Complete**: Celebration haptics + victory sound
- **Tile Tap**: Gentle haptic feedback on every tap

Both sound and haptics can be toggled independently in settings. Works on both iPhone and Apple Watch!

### Grid Sizes
- **2×2**: 4 tiles (faster gameplay, 8s base time)
- **2×4**: 8 tiles (medium, 12s base time)
- **3×5**: 15 tiles (more choices, 15s base time)

### Progressive Difficulty
- Game always starts at Level 1
- Time limit reduces by **15%** per level (factor: 0.85^(Level-1)) - **increased difficulty!**
- Each level consists of **6 rounds**
- Score multiplier increases exponentially with level
- **Game ends immediately on any wrong selection or timeout** - no second chances!

### Scoring System

**Base Points** (per round):
- 2×2 Grid: 10 points
- 2×4 Grid: 14 points
- 3×5 Grid: 18 points

**Multipliers**:
- **Level Multiplier**: 2^(Level-1)
- **Time Multiplier**: Seconds remaining (rounded, minimum 1) ⚡ **NEW!**
- **Shapes Bonus**: 1.2× (20% more points)
- **Emoji Bonus**: 1.15× (15% more points) - **reduced from 30%**
- **Pro Mode Bonus**: 1.5× (50% more points)

**Formula**:

