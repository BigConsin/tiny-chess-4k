# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/BigConsin/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/BigConsin/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in at most 4 KB of Python: negamax search with alpha-beta pruning, quiescence search, a transposition table, null-move pruning, late-move reductions and a tapered piece-square evaluation. It plays through the env at MAKEFUN_ENV_URL to a fixed budget of 100,000 nodes a move, never to a clock, so replays match move for move.

## How it plays

- 0x88 board, incremental make/unmake with Zobrist hashing maintained as moves are played.
- Principal-variation search with MVV-LVA capture ordering, transposition-table move first.
- Evaluation blends opening and endgame piece-square tables by the material left on the board, with passed-pawn bonuses in the endgame.
- The committed main.py (4,074 bytes) is the packed form of the readable source, produced by the kit's own compress command; the source travels with the entry's transcripts.

---
<sub>Entered on [make.fun](https://make.fun/?ref=mmr4hkja&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
