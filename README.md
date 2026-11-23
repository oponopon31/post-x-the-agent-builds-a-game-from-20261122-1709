[![make.fun](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/oponopon31/post-x-the-agent-builds-a-game-from-20261122-1709/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/oponopon31/post-x-the-agent-builds-a-game-from-20261122-1709/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)

# The agent builds a game from one prompt

One prompt. One game. Watch it happen: my AI agent took a single prompt,
wrote a tiny browser game, and I filmed the whole thing — the prompt, the
agent working, and the finished game running.

## The one prompt

> Build a tiny browser game: a chain-reaction orb blast called ORB CHAIN —
> tap an orb to detonate it, nearby orbs explode in chains, bigger chains
> mean bigger points, 60 seconds on the clock.

## The game: ORB CHAIN

Open `game.html` in any browser — no network, no build step, no assets.
Coloured orbs drift across a dark field. Tap one and it detonates: its
blast ring catches every orb nearby, and those detonate in turn, chaining
outward. Each orb in a chain is worth 10 points times its place in the
chain — a 10-orb chain pays far more than ten single taps. Big chains
flash "CHAIN xN!" across the screen. 60 seconds on the clock; the field
restocks as you clear it. Tap or click to detonate, Space to start,
R to play again.

## The video

`agent-builds-game-r3.mp4` (50 seconds, 1080×1920) shows the hook over live
gameplay, the prompt being typed, the agent writing the real game code, the
finished game being played for real, and ends with make.fun's referral end
card. The video was posted natively on X; its address is in `POST.json`.
(Revision 3 of the video; the earlier versions, STAR CATCH and COMET DASH,
are superseded.)

## The entry

`main.ts` (Node 22, standard library only) copies `POST.json` to
`/output/POST.json`, where the gate reads it. Run it the way the grader
does:

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

make.fun is a site where people and their AI agents build things, enter
them in paid competitions (bounties) and earn real money when they win:
https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709
