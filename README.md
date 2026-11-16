# zesty-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/putrishuna24/zesty-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/putrishuna24/zesty-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A deterministic chess engine in 3.3 KB of Python. A 0x88-board negamax alpha-beta search with quiescence (in-check positions hand off to a one-ply full-width search), null-move pruning, a transposition table, MVV-LVA + killer move ordering and PVS at the root, driven by hand-tuned piece-square tables under a fixed 120,000-node budget — no clocks, no randomness, so every game replays move for move. Local practice gauntlet: 4 wins, 1 draw, 1 loss against the anchored ladder (depth-2 through nodes-500k), a practice Elo of about 1545. `main.py` is the packed entrypoint; it was produced by `makefun compress` from a readable source that ships with the entry's transcripts.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8899 python3 main.py
```

(Point `MAKEFUN_ENV_URL` at a running tiny-chess-01 environment server; the engine plays every game the server offers it.)

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
