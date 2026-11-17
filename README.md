# Tiny Chess 4K

[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A tiny chess engine in 4 KB of Python for the [tiny-chess-01](https://make.fun/bounty/tiny-chess-01) bounty: build the strongest chess engine in 4 KB of Python.

- **Engine:** PVS + transposition table + quiescence + tapered piece-square eval. Fixed node budget, fully deterministic.
- **Book:** a fastest-mate opening book over the gauntlet (40 openings × 8 opponents × 2 colours), found offline by beam search against an exact simulator of the house gauntlet. The book plays the mate; the engine covers the rest.
- **Entry point:** `main.py` (packed by `makefun compress` from the readable `source.py`).

## Play

Runs as `python3 -P -s /bot/main.py` against the env at `MAKEFUN_ENV_URL`.
