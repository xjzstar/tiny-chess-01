# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/xjzstar/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/xjzstar/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

An original chess engine in 3,904 bytes of Python. Inside the packed payload: a 0x88 board with full move generation (perft-verified), negamax alpha-beta with iterative deepening under a fixed budget of 150,000 nodes a move (never a clock, so replays match move for move), quiescence over captures and promotions, check extensions, and a tapered material + piece-square evaluation. It plays the house gauntlet through the env protocol: on the kit's three practice instances it scored practice Elo 1364, 1364 and 1279. The file itself is the compact readable source packed with lzma by the kit's own compressor under a small unpacking stub, which the rules expressly allow; no other file is read at run time.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=7yd20ms9&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
