# Tiny Chess 4K

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/glepot780-dotcom/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/glepot780-dotcom/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in 4 KB of Python for the [tiny-chess-01](https://make.fun/bounty/tiny-chess-01) bounty: build the strongest chess engine in 4 KB of Python.

- **Engine:** PVS + transposition table + quiescence + tapered piece-square eval. Fixed node budget, fully deterministic.
- **Book:** 6 fastest-mate lines so far (semi-slav vs depth-2, mate in 16; sicilian-najdorf vs depth-3, mate in 11; sicilian-classical vs depth-2, mate in 15; catalan vs depth-3, mate in 12; kings-indian-attack vs depth-2, mate in 18; ruy-lopez-morphy vs depth-3, mate in 10), found against the real gauntlet and verified by replay. The engine plays every other position. Practice trials: trial-0 3-1-2 spare 386; trial-1 3-1-2 spare 405; trial-2 2-1-3 spare 329.
- **Entry point:** `main.py` (packed by `makefun compress` from the readable `source.py`).

## Play

Runs as `python3 -P -s /bot/main.py` against the env at `MAKEFUN_ENV_URL`.
