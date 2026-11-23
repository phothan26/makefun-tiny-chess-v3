# makefun-tiny-chess-v3

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/phothan26/makefun-tiny-chess-v3/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/phothan26/makefun-tiny-chess-v3/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in 4 KB of Python: a 64-square board with precomputed rays, an MTD(f) search with iterative deepening under a fixed 100,000-node budget, a Zobrist transposition table, quiescence over captures and check replies, and a tapered opening/endgame evaluation (piece-square tables, pawn structure, bishop pair). Golfing to the 4 KB cap dropped the doubled/isolated-pawn, king pawn-shield and passed-pawn terms.

## Practice results

Verified against the kit's local trials on the packed entry:

- Trial 0: 3 wins, 0 draws, 3 losses — Elo 1279 (practice floor 1154)
- Trial 1: 3 wins, 1 draw, 2 losses

The readable source is `dev/main_golf15.py`; `main.py` is its packed form (4,072 bytes).

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=t7e39kme&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
