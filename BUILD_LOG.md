# Soph's Solitaire Build Log

## Initial build

- Created as a separate project so Scholar Slash and its history remain unchanged, then renamed to **Soph's Solitaire**.
- Chose Klondike rules with stock, waste, four foundations, and seven tableau columns.
- Assigned Mac Miller to Jacks, Tana Mongeau to Queens, Flea to Kings, and Tiger Woods to Aces.
- Replaced requested copyrighted press and album images with Creative Commons photographs safe for public reuse.
- Added local assets, visible credits, full attribution, restart/new-deal controls, move tracking, and win detection.

## Full rules audit

- Corrected destination-card clicks so selected cards and stacks move into tableau columns.
- Added click-again and Escape cancellation for mistaken selections.
- Added dynamic board height so long columns cannot overflow or create layout holes.
- Passed browser checks for a unique 52-card deal, 24-card stock, 1-7 tableau deal, stock recycling, alternating-color descending moves, rejection of same-color and rank-gap moves, King-only empty columns, multi-card sequences, automatic reveals, waste moves, ascending same-suit foundations, foundation-to-tableau recovery, win detection, and all four portrait assets.
- Replaced unrestricted random shuffles with varied guaranteed-solvable deals, preventing all four Kings or other required cards from becoming permanently blocked while retaining standard Klondike move rules.
- Completed 100 automated full-game playthroughs from the opening deal through all four Kings; all 100 distinct deals reached the rendered win screen with no missing or duplicate cards.
- Customized the completed-game message to read **Regi is Impressed** with the requested chud-life subtitle.
- Added rule-checked drag-and-drop for tableau stacks, the top waste card, and top foundation cards while preserving click and double-click controls.
- Expanded double-click to automatically choose a legal foundation first or a fitting tableau column for single cards and movable stacks.
- Replaced fragile native `dblclick` handling with persistent card-ID timing so auto-move still triggers when the first click re-renders the card element.
