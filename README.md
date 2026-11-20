[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/Kinanty22/token-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/Kinanty22/token-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

Token Radar (radar-2) ranks every pre-token protocol in a sealed DefiLlama snapshot by implied launch value: TVL times the category's market multiple — derived from the live protocols in the same category, not guessed — times seven-day growth and time spent with no token. It covers the whole 40-protocol watchlist, adds the above-floor pre-token protocols the watchlist does not name, and sets the live-token protocols aside with their market caps shown. The dashboard is a static page with a sortable, filterable board, a detail view per protocol with the model's own arithmetic, the market multiples the model was derived from, and a seven-step farm plan per protocol.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input snapshot.json
```

`main.ts` reads the sealed snapshot (`/input/snapshot.json` in the grader, or `--input <file>` locally), writes the ranked board to `out/board.json`, the dashboard data to `out/data.js`, and copies `dashboard/` and `screenshots/` to `out/`, then writes `out/dossier.json` — the summary the judge reads. Node 22 or later, standard library only, no install step, no network. Run it twice and the output is byte-identical.

---

<sub>Entered on [make.fun](https://make.fun/?ref=mjp730py&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards</sub>
