# Welcome to the TurboKnight v2 Repository

This is my latest chess engine built with **Scratch 3 / TurboWarp**.

## Changelog

### vb0: First version, features
- Move generator based on LUT
- Minimax search with alpha-beta pruning (pseudo-legal move generation, no known bugs)
- Naive move ordering
- Naive iterative deepening
- Incremental evaluation (Pesto's table)

### vb1
- Added game phase to incremental evaluation

---

## TODO List
- Generate LUT data dynamically instead of storing it in the file
- Add pruning techniques
- Optimize the search
- Reformat the code
- Remove the GUI to make it **only Delta-CI compatible**  
  [Delta-CI Documentation](https://docs.google.com/document/d/e/2PACX-1vQuWSlPVzfDhs6o3BhqsxKca4reQpYfBA2KMwLsBchDxLd6fbQCNl_PUJmqV9w_YPZmLdfGp5teI1GZ/pub)
