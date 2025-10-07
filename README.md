# ♞ TurboKnight v2

**TurboKnight v2** is my latest chess engine, built with **Scratch 3 / TurboWarp**.  
It aims to push the limits of what’s possible in a visual programming environment while implementing modern search and evaluation techniques.

---

## 📌 Table of Contents
- [Features](#features)
- [Changelog](#changelog)
- [TODO / Roadmap](#todo--roadmap)
- [Build & Compatibility](#build--compatibility)
- [Credits & Links](#credits--links)

---

## ⚙️ Features

- Move generation based on **LUT**
- **Minimax search** with alpha–beta pruning
- **Incremental PST evaluation** (based on Pesto’s tables)
- **LMR** (Late Move Reductions)
- **Aspiration windows**
- **SEE** (Static Exchange Evaluation) move ordering
- **Dynamic LUT generation** (no static tables)
- Support for **Delta-CI** testing interface *(work in progress)*

---

## 🧾 Changelog

### 🔸 vb0 – Initial Release
- Move generator (LUT-based)
- Minimax with alpha–beta pruning (pseudo-legal)
- Naive move ordering and iterative deepening
- Incremental eval (Pesto’s table)
- Basic LMR

### 🔸 vb1
- Added game phase to incremental evaluation

### 🔸 vb2
- Removed 3-repetition detection (too slow)
- Will be reimplemented later with new ideas

### 🔸 vb3
- Fixed LMR re-search logic (`score > alpha` / `< beta`)
- Added ZWP (Zero-Window Pruning)
- Improved move ordering (SEE)
- More stable search

### 🔸 vb16
- Fixed bugs in `king_in_check`
- Improved LMR and aspiration windows
- Added search extensions
- Switched to fully legal move generation
- Added dynamic LUT generation
- Removed ZWP (too slow)
- General move ordering improvements

---

## ✅ TODO / Roadmap

### 🔹 Search Improvements
- [ ] Delta pruning  
- [ ] Null Move Pruning (NMP)  
- [ ] Futility pruning  
- [ ] Extended futility pruning  
- [ ] Re-add and optimize ZWP (currently slower)  
- [ ] Transposition Tables  

### 🔹 Evaluation
- [x] Fully incremental PST-based evaluation  
- [ ] Pawn structure evaluation  
- [ ] King safety evaluation  
- [ ] Attack / proximity evaluation (e.g. enemy queen near king)  

### 🔹 Engine & Integration
- [x] Generate LUT dynamically (instead of static file)  
- [ ] Optimize NPS (nodes per second)  
- [ ] Reformat and clean codebase  
- [ ] Remove GUI — make it **Delta-CI compatible only**  

---

## 🧰 Build & Compatibility

| Environment | Status |
|--------------|--------|
| **Scratch 3** | ✅ Supported (no turbowarp-only blocks) |
| **TurboWarp** | ✅ Optimized |
| **Delta-CI** | ⚙️ Planned (no GUI mode) |

📘 [Delta-CI Documentation](https://docs.google.com/document/d/e/2PACX-1vQuWSlPVzfDhs6o3BhqsxKca4reQpYfBA2KMwLsBchDxLd6fbQCNl_PUJmqV9w_YPZmLdfGp5teI1GZ/pub)

---

## 🙌 Credits & Links

- **Evaluation tables:** [Pesto’s tables](https://www.chessprogramming.org/Simplified_Evaluation_Function)
- **Inspired by:** Arnohu's scratch chess engine, and all other ones 
- **Made with:** Turbowarp desktop

---

> “A chess engine written in blocks, but built like a real one.”
