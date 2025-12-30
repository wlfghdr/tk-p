---
name: Platform Consistency Issue
about: Report inconsistencies between iOS and watchOS implementations
title: '[CONSISTENCY] '
labels: platform-consistency, bug
assignees: ''

---

## 🔴 Platform Consistency Issue

<!-- This template is for reporting differences in behavior between iOS and watchOS that should be consistent -->

## 📝 Description

<!-- Clear description of the inconsistency between platforms -->

## 📱 Affected Platforms

<!-- Which platforms are affected? -->

- [ ] iOS behaves differently than watchOS
- [ ] watchOS behaves differently than iOS
- [ ] One platform missing feature present on the other

## 🎮 Area Affected

<!-- What aspect of the game is inconsistent? -->

- [ ] Scoring calculation
- [ ] Level progression
- [ ] Timer behavior
- [ ] Tile generation
- [ ] Game over conditions
- [ ] Round/level mechanics
- [ ] UI/UX elements
- [ ] Settings/configuration
- [ ] Localization
- [ ] Other (describe below)

## 🔍 Current Behavior

### iOS Behavior

<!-- Describe what happens on iOS -->

**Steps to reproduce on iOS:**
1. 
2. 
3. 

**iOS Result:**


### watchOS Behavior

<!-- Describe what happens on watchOS -->

**Steps to reproduce on watchOS:**
1. 
2. 
3. 

**watchOS Result:**


## ✅ Expected Behavior

<!-- What should the consistent behavior be across both platforms? -->

## 📸 Screenshots/Comparisons

### iOS Screenshot

<!-- Add iOS screenshot here -->

### watchOS Screenshot

<!-- Add watchOS screenshot here -->

## 🧪 Test Cases

<!-- Describe how to verify the inconsistency -->

### Test on iOS
```
1. [Step 1]
2. [Step 2]
3. [Step 3]
Expected: [Expected result]
Actual: [Actual result]
```

### Test on watchOS
```
1. [Step 1]
2. [Step 2]
3. [Step 3]
Expected: [Expected result]
Actual: [Actual result]
```

## 📋 Environment

### iOS
- **Device**: [e.g., iPhone 15]
- **iOS Version**: [e.g., iOS 17.2]
- **App Version**: [e.g., 1.0]

### watchOS
- **Device**: [e.g., Apple Watch Series 9]
- **watchOS Version**: [e.g., watchOS 10.2]
- **App Version**: [e.g., 1.0]

## 🎮 Game Settings

<!-- Settings used when inconsistency was discovered -->

- **Game Mode**: [Colors / Emojis]
- **Grid Size**: [2×2 / 2×4 / 3×4 / Fixed 2×2 on watchOS]
- **Pro Mode**: [ON / OFF]
- **Language**: [German / English]
- **Theme**: [Light / Dark / System]
- **Start Level**: [e.g., 1]

## 🔢 Game State

<!-- Game state when inconsistency occurred -->

- **Level**: [e.g., Level 5]
- **Round**: [e.g., Round 3 of 6]
- **Score**: [e.g., iOS: 240, watchOS: 200]
- **Time Remaining**: [e.g., iOS: 3.5s, watchOS: 4.0s]

## 📝 Code Investigation

<!-- If you've looked at the code, note differences here -->

### iOS Implementation

**File**: `Timekiller/ContentView_iOS.swift`  
**Line**: [Line number or range]

```swift
// Paste relevant iOS code here
```

### watchOS Implementation

**File**: `Timekiller Watch App/ContentView.swift`  
**Line**: [Line number or range]

```swift
// Paste relevant watchOS code here
```

### Difference Analysis

<!-- What's different in the implementations? -->

## 🤔 Valid or Invalid Inconsistency?

<!-- Some differences are valid due to screen constraints -->

### Is this difference justified?

- [ ] **Invalid** - Should be identical across platforms
- [ ] **Valid** - Difference justified by platform constraints
- [ ] **Uncertain** - Need clarification

### Justification (if valid)

<!-- If you think the difference is valid, explain why -->
<!-- Example: "watchOS has limited screen space and can't display 3×4 grid" -->

## 💭 Proposed Solution

<!-- How should this inconsistency be resolved? -->

### Option 1: Make Identical

<!-- Make both platforms behave the same -->

**Changes needed:**
- [ ] Update iOS implementation to match watchOS
- [ ] Update watchOS implementation to match iOS
- [ ] Create consistent shared logic in GameModels.swift

### Option 2: Document Exception

<!-- If difference is valid, document it -->

**Documentation updates needed:**
- [ ] Add comment in iOS code explaining difference
- [ ] Add comment in watchOS code explaining difference
- [ ] Update CLAUDE.md with exception
- [ ] Update REQUIREMENTS.md if needed

## 📚 Related Documentation

<!-- Which docs discuss this area? -->

- [ ] REQUIREMENTS.md - Section: [Section name]
- [ ] CLAUDE.md - Section: [Section name]
- [ ] README.md - Section: [Section name]

## 🔗 Related Issues

<!-- Link to related issues if any -->

Related to #

## 🎯 Impact Assessment

### Severity

- [ ] Critical - Breaks core gameplay
- [ ] High - Significant inconsistency affecting experience
- [ ] Medium - Noticeable but not game-breaking
- [ ] Low - Minor inconsistency

### User Impact

- [ ] Players notice and are confused
- [ ] Affects game fairness
- [ ] Affects highscores/scoring
- [ ] Affects learning curve
- [ ] Visual/cosmetic only

## ✅ Verification Checklist

<!-- For fixes: How to verify the issue is resolved -->

- [ ] Test identical behavior on iOS
- [ ] Test identical behavior on watchOS
- [ ] Test with Colors mode
- [ ] Test with Emojis mode
- [ ] Test with different grid sizes
- [ ] Test with Pro mode ON/OFF
- [ ] Test in both German and English
- [ ] Verify documentation updated
- [ ] Verify comments added to code

---

**For Contributors:**

When fixing this inconsistency:
1. **Verify the inconsistency** exists on both platforms
2. **Determine if difference is valid** (screen size constraints)
3. **If invalid**: Make implementations identical
   - Update both ContentView files
   - Extract to shared GameModels if appropriate
   - Test on both platforms
4. **If valid**: Document the exception
   - Add comments in both files
   - Update CLAUDE.md
   - Explain reasoning clearly
5. **Update documentation** to reflect resolution
6. **Follow PR template** for platform consistency

### Core Principle

**Game logic (scoring, timing, progression) must be identical across platforms.**  
**Only UI/layout should differ due to screen constraints.**
