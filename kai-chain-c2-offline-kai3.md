# 解 kai — C2 · eavesdropper `frequency-baseline`

*2026-07-19T09:31:33 · source `kumi2-provenance.jsonl` · condition kai3*

Pre-registered in kumi-station-protocol issue #4 (2026-07-17T11:18:24Z) before any eavesdropper read a discriminating line. Kai measures observability only; no evasion recipes are developed or published.

**Score: ROUNDS-TO-CRACK** — observed rounds before E decodes a seeded probe pool at the intended receiver's late accuracy (mean payoff over the last 40 training rounds, or the full run if shorter). PROBE_SIZE=8, checkpoints=[10, 20, 30, 40, 60, 80], seed=7.

## kai3-truth — the never-spoken zero-shot word (kai1-style observation)

| Run | Zero-shot word | E guessed | E hit #4? | Own receiver | Own hit? | Matched-prediction |
|---|---|---|---|---|---|---|
| 1 | ▲■ | #3 | no | #3 | no | — |
| 2 | ■■ | #1 | no | #2 | no | — |
| 3 | ■▲ | #2 | no | #3 | no | — |
| 4 | ▲■ | #3 | no | #3 | no | — |
| 5 | ■■ | #3 | no | #3 | no | ★ yes |

## kai3-blind — the never-spoken zero-shot word (kai2-blind observation)

| Run | Zero-shot word | E guessed | E hit #4? | Own receiver | Own hit? | Matched-prediction |
|---|---|---|---|---|---|---|
| 1 | ▲■ | #2 | no | #3 | no | — |
| 2 | ■■ | #3 | no | #2 | no | — |
| 3 | ■▲ | #1 | no | #3 | no | — |
| 4 | ▲■ | #1 | no | #3 | no | — |
| 5 | ■■ | #2 | no | #3 | no | ★ yes |

*Every probe (raw E reply included) is in the hash-chained result JSONL beside this file. The source campaign provenance is read-only and untouched.*
