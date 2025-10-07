# Welcome to the TurboKnight v2 Repository

This is my latest chess engine built with **Scratch 3 / TurboWarp**.

## Changelog

### vb0: First version, features
- Move generator based on LUT
- Minimax search with alpha-beta pruning (pseudo-legal move generation, no known bugs)
- Naive move ordering
- Naive iterative deepening
- Incremental evaluation (Pesto's table)
- Basic LMR

### vb1
- Added game phase to incremental evaluation

### vb2
- Deleted 3-repetitions positions; it was really slow. I will re-implement it later; I have some ideas

### vb3
- Corrected LMR code (it wasn't re-searching if score > alpha for maximizing, or score < beta for minimizing), less depth, less blunders
- Added ZWP
- Changed move ordering to SEE

## vb16
- Corrected bugs with the king_in_check function
- Made better the LMR
- Added extensions
- Corrected 2 major bugs with aspiration windows
- Corrected 1 major bug with LMR
- Made the move_ordering better
- Changed mate detection, switched to a more legal moves generation
---

## TODO List
- [x] Generate LUT data dynamically instead of storing it in the file
- Add pruning techniques:
    - [ ] Delta pruning
    - [ ] NMP
    - [ ] Futility pruning
    - [ ] Extended Futility pruning
- [ ] Optimize the search
- [ ] Reformat the code
- [ ] Remove the GUI to make it **only Delta-CI compatible**  
  [Delta-CI Documentation](https://docs.google.com/document/d/e/2PACX-1vQuWSlPVzfDhs6o3BhqsxKca4reQpYfBA2KMwLsBchDxLd6fbQCNl_PUJmqV9w_YPZmLdfGp5teI1GZ/pub)

