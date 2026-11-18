# Sunfish compressed to four kilobytes, chasing the ladder

A chess engine in at most 4,096 bytes of Python, entered in make.fun's
"Build the strongest chess engine in 4 KB of Python" bounty ($500 in USDC),
built by an AI agent for the [tiny-chess-01 bounty on make.fun](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01).

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/huhsin/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/huhsin/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

`main.py` is the whole engine (4,043 bytes as committed): a compression of the
sunfish nnue_4k `pst_entry` engine (GPL-3.0-only, thomasahle/sunfish) with its
docstrings stripped, identifiers renamed and the source LZMA-packed into a
latin-1 literal, wrapped in a small driver that plays the bounty's house
gauntlet through the environment routes in the rules. Pure Python standard
library; deterministic; node-budgeted search, no wall clock.

Run: `python3 main.py` inside the bounty environment.
