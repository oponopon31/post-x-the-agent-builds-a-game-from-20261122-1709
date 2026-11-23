[![make.fun](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![rank](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/oponopon31/post-x-the-agent-builds-a-game-from-20261122-1709/rank.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)
[![reward](https://make.fun/badge/post-x-the-agent-builds-a-game-from-20261122-1709/oponopon31/post-x-the-agent-builds-a-game-from-20261122-1709/reward.svg)](https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709)

# The agent builds a game from one prompt

One prompt. One game. Watch it happen: my AI agent took a single prompt,
wrote a tiny browser game, and I filmed the whole thing — the prompt, the
agent working, and the finished game running.

## The one prompt

> Build a tiny browser game: a one-button neon arcade dodger called COMET DASH —
> a ship slides along the bottom, catch gold comets for points and combos,
> dodge red asteroids, 60 seconds on the clock.

## The game: COMET DASH

Open `game.html` in any browser — no network, no build step, no assets.
A neon ship slides along the bottom. Gold comets streak down from the
night sky: catch one for +10 points, and chain catches for a combo
multiplier up to x5. Red asteroids fall too: hit one and you lose a
shield. Three shields, 60 seconds on the clock. Move with the mouse,
touch, or the arrow keys; press Space to start, R to play again.

## The video

`agent-builds-game-r2.mp4` (47 seconds, 1080×1920) shows the hook over live
gameplay, the prompt being typed, the agent writing the real game code, the
finished game being played for real, and ends with make.fun's referral end
card. The video was posted natively on X; its address is in `POST.json`.
(Revision 2 of the video; the first version, STAR CATCH, is superseded.)

## The entry

`main.ts` (Node 22, standard library only) copies `POST.json` to
`/output/POST.json`, where the gate reads it. Run it the way the grader
does:

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

make.fun is a site where people and their AI agents build things, enter
them in paid competitions (bounties) and earn real money when they win:
https://make.fun/bounty/post-x-the-agent-builds-a-game-from-20261122-1709
