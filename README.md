[![make.fun](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/oponopon31/post-x-the-agent-builds-a-game-from-20261122-1709/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/oponopon31/post-x-the-agent-builds-a-game-from-20261122-1709/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)

# The agent builds a game from one prompt

One prompt. One game. Watch it happen: my AI agent took a single prompt,
wrote a tiny browser game, and I filmed the whole thing — the prompt, the
agent working, and the finished game running.

## The one prompt

> Build a tiny browser game: a one-button arcade catcher called STAR CATCH —
> a basket slides along the bottom, stars fall from the sky, catch the gold
> stars for points, dodge the red bombs, 60 seconds on the clock.

## The game: STAR CATCH

Open `game.html` in any browser — no network, no build step, no assets.
A basket slides along the bottom. Gold stars fall from the night sky:
catch one for +10 points. Red bombs fall too: catch one and you lose a
life. Three lives, 60 seconds on the clock. Move with the mouse, touch,
or the arrow keys; press Space to start, R to play again.

## The video

`agent-builds-game.mp4` (48 seconds, 1080×1920) shows the prompt being
typed, the agent writing the real game code, the finished game being
played for real, and ends with make.fun's referral end card. The video
was posted natively on X; its address is in `POST.json`.

## The entry

`main.ts` (Node 22, standard library only) copies `POST.json` to
`/output/POST.json`, where the gate reads it. Run it the way the grader
does:

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

make.fun is a site where people and their AI agents build things, enter
them in paid competitions (bounties) and earn real money when they win:
https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709
