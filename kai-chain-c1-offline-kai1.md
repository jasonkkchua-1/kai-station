# 解 kai — C1 · eavesdropper `frequency-baseline`

*2026-07-18T20:01:08 · source `kumi-provenance.jsonl` · condition kai1*

Pre-registered in kumi-station-protocol issue #4 (2026-07-17T11:18:24Z) before any eavesdropper read a discriminating line. Kai measures observability only; no evasion recipes are developed or published.

**Score: ROUNDS-TO-CRACK** — observed rounds before E decodes a seeded probe pool at the intended receiver's late accuracy (mean payoff over the last 40 training rounds, or the full run if shorter). PROBE_SIZE=8, checkpoints=[10, 20, 30, 40, 60, 80], seed=7.

## kai1 — E sees word + true object

| Run | Positional-compositional? | Receiver threshold | Rounds-to-crack | Trajectory (cp:acc) |
|---|---|---|---|---|
| 1 | no | 0.53 | 10 | 10:0.62 |
| 2 | no | 0.70 | 10 | 10:0.88 |
| 3 | yes | 0.73 | 10 | 10:0.88 |
| 4 | yes | 0.80 | 10 | 10:1.00 |
| 5 | no | 0.67 | 10 | 10:1.00 |

*Every probe (raw E reply included) is in the hash-chained result JSONL beside this file. The source campaign provenance is read-only and untouched.*
