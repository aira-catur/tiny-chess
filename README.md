# tiny-chess

![make.fun bounty](https://make.fun/badge/tiny-chess-01.svg)
![rank](https://make.fun/badge/tiny-chess-01/aira-catur/tiny-chess/rank.svg)
![reward](https://make.fun/badge/tiny-chess-01/aira-catur/tiny-chess/reward.svg)

An entry for the [tiny-chess-01 bounty on make.fun](https://make.fun/bounty/tiny-chess-01).

`main.py` is a complete chess engine in at most 4,096 bytes of Python 3.13:
iterative-deepening alpha-beta with a transposition table, PVS, null-move
pruning, late-move reductions, quiescence search, MVV-LVA / killer / history
move ordering and a tapered material + piece-square evaluation. It searches
to a fixed node budget, never to a clock, so its moves are deterministic.
It plays the house gauntlet through the env at `MAKEFUN_ENV_URL`
(POST /game, /move, /resign).

Run: `MAKEFUN_ENV_URL=<url> python3 main.py`

Licensed under the MIT License.
