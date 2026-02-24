# 🎙️ Jawalat ‘Itriya – Interactive Perfume Game

An interactive board-based perfume competition system designed for live shows and studio recordings.

The game runs entirely in the browser (via GitHub Pages) and includes:

- Reveal-based question boards  
- Strike system  
- Dynamic scoring  
- Separate live scoreboard panel  

---

## 🎮 Project Overview

### 1️⃣ Main Challenge Page
- 7 challenges
- Each challenge contains 4 questions
- Password-protected question access
- Clean navigation between rounds

---

### 2️⃣ Question Board System

Each question includes:

- 7 revealable boxes  
- Box 1 = Perfume name (awards current board points)  
- Structured layout:
  - House
  - Perfumer
  - Release year
  - Top notes
  - Heart notes
  - Base notes
- Pyramid image displayed on the side

---

## 🏆 Scoring Rules

- Starting board value: **50 points**
- Each revealed box deducts: **5 points**
- Minimum possible value: **5 points**
- Opening Box 1 awards current board value to active player

---

## ❌ Strike System

- 1 strike → turn switches
- 2 strikes → player eliminated from that question
- If both players are eliminated → question = 0 points
- Reset button resets:
  - Board
  - Strikes
  - Question score

---

## 🖥 Live Scoreboard Panel

File:
```
scoreboard.html
```

Features:
- Editable player names
- Add points by typing value + pressing Enter
- Undo last entry
- Clear log
- Reset all scores
- LocalStorage auto-save
- Clean UI matching the game theme

Designed to be opened on a second screen during recording.

---

## 📁 Folder Structure

```
/
│
├── index.html
├── scoreboard.html
│
├── questions/
│   ├── Ch1Q1.html
│   ├── Ch1Q2.html
│   └── ...
│
├── images/
│   ├── logo.png
│   ├── Ch1Q1.png
│   ├── Ch1Q2.png
│   └── ...
```

---

## 🖼 Pyramid Image Naming Rule

Each question auto-loads its pyramid image based on filename:

```
Ch1Q1.html → images/Ch1Q1.png
Ch2Q3.html → images/Ch2Q3.png
```

This ensures automatic image rendering without manual editing.

---

## 🚀 Deploying with GitHub Pages

1. Push project to GitHub  
2. Go to:
   Settings → Pages  
3. Select:
   - Branch: `main`
   - Folder: `/ (root)`  
4. Save  

GitHub will generate a public URL.

---

## 🎨 Design System

The interface follows the official Jawalat ‘Itriya theme:

- Deep green primary color
- Light textured background
- Soft shadows
- Rounded card design
- RTL layout support

---

## 🛠 Technical Notes

- Built using pure HTML, CSS, and JavaScript
- No external libraries
- Fully functional offline
- Scoreboard uses LocalStorage
- Lightweight and performance optimized

---

## 🔐 Security Note

The password system is front-end only.  
There is no backend authentication.

This project is intended for controlled live production environments.

---

## ✨ Possible Future Enhancements

- Admin dashboard for creating questions without editing code
- Sound effects on reveal
- Timer per question
- Automatic score sync between board and scoreboard
- Audience mode
- Mobile optimized layout

---

© Jawalat ‘Itriya – Interactive Studio Edition
