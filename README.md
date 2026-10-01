# Snail Patrol

You're the lead duck on a South African wine farm. The vines are crawling with snails. Clear them before the rain, without a drop of pesticide.

**[Play it](https://dondino-go.github.io/snail-patrol/)** · **[The hackathon pitch](https://dondino-go.github.io/snail-patrol/pitch.html)** · or clone the repo and open `index.html`. There's no build step and no dependencies.

Inspired by [Vergenoegd Löw](https://www.rte.ie/news/newslens/2026/0822/1588801-ducks-south-african-wine-farm/), a wine estate near Stellenbosch where about 1,000 Indian Runner ducks eat the snails off the vines instead of the farm using pesticides.

## Controls

| | |
|---|---|
| Arrows / WASD | steer the line (it keeps going until it can turn) |
| `Space` | send the back half of your line off on patrol |
| `Q` | Big Quack (once you've earned it) |
| `1`–`4` | pick tonight's upgrade |
| `M` | mute |

On a phone: swipe to steer, tap to send a patrol.

## The rules

- Every block starts infested. Any duck that walks past a snail eats it. Clear every snail before time runs out; seconds to spare become bonus bottles.
- Every duck behind you slows you down. Patrols are dumb on purpose: they mow the rows in a zig-zag and stop dead in puddles. Walk into a patrol to take it back.
- Rain brings fresh snails onto rows you've already cleared.
- Five days, five blocks, one upgrade each night, then the harvest.

This is a grey-box prototype. All the tuning numbers are at the top of the `<script>` in `index.html`.

## Docs

- [`BACKLOG.md`](BACKLOG.md): what we've tried, what we learned, and ideas to explore
- [`PLAYTEST.md`](PLAYTEST.md): how to run a playtest
- [`PITCH.md`](PITCH.md): the hackathon pitch in text, with a Slack post ready to paste
