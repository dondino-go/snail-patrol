# Backlog: ideas to explore

These are ideas, not commitments, and not a roadmap. Pull from here when you're choosing the next thing to build.

---

## What we've learned so far

| Version | What it tried | Verdict |
|---|---|---|
| v1 | Free-moving flock defends the vines from snails that keep spawning | The flock was just a wide brush. A bigger flock felt like no gain. |
| v2 | Grid maps, Pac-Man movement, splitting off dumb patrols, a longer line slows you | Interesting, but defending against random spawns felt like whack-a-mole |
| v3 | **Restore, not defend:** the block starts infested, you clear it fast, rain re-infests | Clearing rows feels great. The loop became *"can I clear it before the next rain?"* |

Keep these: clearing rows, combos, "Row saved!", the rain deadline, and one block per day.

---

## 1. Patrols (the next big thing to work on)

Being slow alone versus sending out dumb patrols is a real trade-off, but it isn't working yet.

- **Aim when you split.** The patrol goes in whichever arrow is held when you press Space, not the way the line was walking. They're just as dumb afterwards, but you get one moment of control. This is the cheapest change to try first.
- **Choose how many to send.** Tap Space to send 1 duck, hold it to send half, or something similar. Right now it's always half.
- **Bigger patrols are slower but sturdier.** A patrol loses one duck to a puddle and keeps going. A lone duck stops dead.
- **Patrols come home.** After one full pass, a patrol waddles back to the leader. Less babysitting, but less control.
- **Signposts (Lemmings).** Drop a sign on a junction and patrols turn there. We deliberately left this out to keep patrols "completely dumb". Revisit if aiming isn't enough.
- **Show where a patrol will go.** A faint dotted line of its next few tiles. Makes the dumb rule readable.
- **The maze problem.** The zig-zag rule only covers about 16% of *The maze*. Decide whether that's a fun "patrols are bad here" day or just annoying.

## 2. Rain as the deadline

This is the pressure players actually feel, so make it the star.

- Make the next shower obvious: a countdown, clouds rolling in from one edge, ducks looking up.
- Maybe drop the 90s timer and let **the rains be the clock**: clear before rain #1 for gold, before rain #2 for silver.
- Rain could re-infest in a visible pattern (one side of the block first) so players can plan for it.
- Forecast at night: *"Tomorrow: heavy rain at 30s"* changes which upgrade you pick.

## 3. Feel and juice

- Duck footsteps, a waddle bob, a squash on each peck
- Combo milestones (x10, x25) with a little fanfare and a duck that does a happy hop
- *BLOCK CLEAR!* that's bigger: confetti, the whole flock quacks in unison
- Screen-shake-lite on Big Quack
- Unique quack voices per duck. A duckling peep.

## 4. Content and hazards

- More maps (we have 5). A map editor, or Tiled, so non-coders can make them.
- **A "ghost"**, as in Pac-Man: the farm dog that scatters the line, a mongoose, or a heron that steals ducklings
- **Tourists on the duck parade** (it's a real tourist attraction at the farm): they block paths, and dropping a snail near them scores style points
- Different snails: big ones that need two pecks, fast ones, ones that hide under leaves
- Aphids or worms as smaller "dots" (the real ducks eat these too)
- The terrace with the cheese board: a Goose-game mischief bonus

## 5. The Stardew layer (keep it light)

- One estate that grows over a season: unlock blocks and see your farm map fill in
- Sell the wine at the market: name your vintage and design the label
- Ducks with names and stats (fast, greedy, easily distracted). Pick who goes on patrol.
- Regenerative farm extras from the real story: sheep and cattle manure, ducks at the irrigation dams once the grapes ripen
- Seasons: harvest, winter pruning, spring hatchlings

## 6. Platforms and access

- Phone: landscape lock, swipe to steer, tap to split (already partly there). Needs testing on a real device.
- Wrap with Capacitor like Bowl Bandit's roadmap, once the loop is proven
- Colour-blind check on snail colours, which currently tell rain snails from dawn snails
- A left-handed or remappable keyboard layout

## 7. Tech and testing

- Host a playable link (GitHub Pages, like Bowl Bandit) for playtests
- Lightweight playtest logging: per-day clear time, bottles, splits, stuck patrols, shown at the end so testers can screenshot it
- Move the bot/balance sims from a scratch folder into `tests/`, Bowl Bandit style
- Art pipeline: real pixel art sprites replace the half-res shapes

---

## Parked (tried or considered, not now)

- **Defend mode** (v1/v2): random spawns all day. Felt like whack-a-mole.
- **Vampire Survivors mode**: an auto-attack aura and a horde. A different game. We kept a taste of it as Big Quack.
- **Duck Tycoon**: selling wine as the main loop. Too big for bite-size.
- **Marigolds upgrade**: meaningless once snails start on the grapes.
