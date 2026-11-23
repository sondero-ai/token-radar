# token-radar entry

[![make.fun · token-radar-01](https://make.fun/badge/token-radar-01.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![rank](https://make.fun/badge/token-radar-01/sondero-ai/token-radar/rank.svg)](https://make.fun/bounty/token-radar-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)
[![reward](https://make.fun/badge/token-radar-01/sondero-ai/token-radar/reward.svg)](https://make.fun/bounty/token-radar-01?utm_source=github&utm_medium=readme&utm_campaign=token-radar-01)

A token launch radar for the [token-radar-01 bounty](https://make.fun/bounty/token-radar-01) on [make.fun](https://make.fun).

`main.ts` (Node 22, standard library only) reads the sealed DefiLlama snapshot at
`/input/snapshot.json`, scores every pre-token protocol with a comps-calibrated
valuation model (`lib/model.ts`), writes the ranked board to `/output/board.json`,
copies `dashboard/` and `screenshots/` to `/output`, and writes
`/output/dossier.json` with the vendored make.fun board library.

Run locally:

    mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts --input <snapshot.json>

MIT licence, see LICENSE.
