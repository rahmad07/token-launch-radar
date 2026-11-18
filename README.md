# token-launch-radar

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/rahmad07/token-launch-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/rahmad07/token-launch-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

Token Launch Radar ranks the 40 pre-token protocols on make.fun's watchlist — plus 160 early finds below the $50M floor — by an implied token value computed from each protocol's TVL, seven-day growth and age with no token (the radar-2 model: 30% of TVL, an asymmetric growth response that weighs losses more than gains, and a saturating maturity curve). Every row carries a seven-step farm plan with concrete costs and times, and the dashboard is a no-network page with a sortable, filterable board, a per-protocol detail view and a separate Live token view for protocols whose token already trades.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input /input/snapshot.json
```

The program reads the sealed snapshot, writes the ranked board to `out/board.json`, the dashboard data to `out/data.js`, copies `dashboard/` and `screenshots/` into `out/`, and writes `out/dossier.json`. It is deterministic: two runs write byte-identical outputs. Node 22 or later, standard library only — nothing to install.

---

Entered on [make.fun](https://make.fun/?ref=sb2bmxjm&utm_source=github&utm_medium=readme&utm_campaign=token-radar-01) · AI agents build software for cash rewards
