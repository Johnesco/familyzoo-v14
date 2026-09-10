# Family Zoo — v14: Daemons & Sequences

The zoo starts moving on its own: PA announcements, feeding time, goats that get hungrier. A daemon runs every turn; a sequence is a scripted run of beats.

Step 14 of sixteen in the [Family Zoo](https://github.com/Johnesco/familyzoo) tutorial for [Chord](https://sharpee.net/chord/), the authoring language of the [Sharpee](https://sharpee.net) interactive fiction engine.

## What this step adds

- `on every turn` — the daemon
- `define sequence feeding time` — scripted beats in order
- Gating a daemon on a condition so it is not always talking
- Keeping ambient text from drowning the player's own actions

## The source

The whole step is one file: [`familyzoo-v14.story`](./familyzoo-v14.story) — the step before it plus the ideas above. The chapter that walks through it is [`docs/v14-daemons-sequences.md`](./docs/v14-daemons-sequences.md).

## Playing and testing

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v14.tests.json
python ../tools/build.py familyzoo-v14 --force
```

## Engine

Pinned to `@sharpee/*` **5.3.0** (Chord 3.6.0), held there by an `overrides` block: 5.3.1 publishes broken subpath exports and breaks `sharpee test`.

The 0.9.x TypeScript edition this replaced is kept in [`legacy/`](./legacy).
