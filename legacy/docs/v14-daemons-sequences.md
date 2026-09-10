# v14 — Daemons & Sequences

The zoo starts moving on its own: PA announcements, feeding time, goats that get hungrier. A daemon runs every turn; a sequence is a scripted run of beats.

## What this step adds

- `on every turn` — the daemon
- `define sequence feeding time` — scripted beats in order
- Gating a daemon on a condition so it is not always talking
- Keeping ambient text from drowning the player's own actions

## The source

The whole step is one file: [`familyzoo-v14.story`](../familyzoo-v14.story). Read it top to bottom — it is the previous step plus what is listed above.

## Running it

```bash
npx sharpee play
npx sharpee test          # replays familyzoo-v14.tests.json
```

Chord language reference: <https://sharpee.net/chord/>
