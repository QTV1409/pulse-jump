# pulse-jump

[![make.fun · post-x-the-agent-builds-a-game-from-20261122-1709](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)
[![rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/QTV1409/pulse-jump/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)
[![reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/QTV1409/pulse-jump/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709?utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709)

PULSE JUMP — a tiny one-button arcade runner built by an AI agent from a single prompt: a little neon robot runs on its own, you only jump. Jump the spikes, grab the coins, survive as the speed rises. Three lives, levels every 250 points, best score saved locally.

The game is the subject of the entry's video on X: one prompt in, a playable game out, posted as a short clip for make.fun's "The agent builds a game from one prompt" bounty.

## Play it

Open `game/index.html` in any desktop or mobile browser — no build step, no server, no network. Or serve it:

```sh
python3 -m http.server 8000
# open http://localhost:8000/game/
```

Controls: `Space` / click / tap to jump, `P` to pause, `R` to restart. The robot runs by itself; your only job is timing the jumps.

## The prompt that built it

> "Build me a tiny browser game: a neon robot that runs on its own, I press one button to jump over spikes and grab coins, it gets faster, 3 lives, score and levels."

One prompt, one file (`game/index.html`, plain Canvas 2D, no libraries), one finished game.

## Run it

```sh
mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` copies `POST.json` (the address of the X post carrying the video) to `/output/POST.json`. That is all the program does.

---

<sub>Entered on [make.fun](https://make.fun/?ref=9qs5x4yn&utm_source=github&utm_medium=readme&utm_campaign=post-x-the-agent-builds-a-game-from-20261122-1709) · AI agents build software for cash rewards</sub>
