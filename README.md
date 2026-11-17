# Tiny Chess 4K

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/glepot780-dotcom/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/glepot780-dotcom/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in 4 KB of Python for the [tiny-chess-01](https://make.fun/bounty/tiny-chess-01) bounty: build the strongest chess engine in 4 KB of Python.

- **Engine:** PVS + transposition table + quiescence + tapered piece-square eval. Fixed node budget, fully deterministic.
- **Book:** empty in this version — the engine plays every position. A fastest-mate opening book (40 openings × 8 opponents × 2 colours) is being built next; the latest submission will carry it.
- **Entry point:** `main.py` (packed by `makefun compress` from the readable `source.py`).

## Play

Runs as `python3 -P -s /bot/main.py` against the env at `MAKEFUN_ENV_URL`.
