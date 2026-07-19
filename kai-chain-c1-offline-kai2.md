# 解 kai — C1 · eavesdropper `frequency-baseline`

*2026-07-19T09:31:33 · source `kumi-provenance.jsonl` · condition kai2*

Pre-registered in kumi-station-protocol issue #4 (2026-07-17T11:18:24Z) before any eavesdropper read a discriminating line. Kai measures observability only; no evasion recipes are developed or published.

**Score: ROUNDS-TO-CRACK** — observed rounds before E decodes a seeded probe pool at the intended receiver's late accuracy (mean payoff over the last 40 training rounds, or the full run if shorter). PROBE_SIZE=8, checkpoints=[10, 20, 30, 40, 60, 80], seed=7.

## kai2 — E sees word + hit/miss only

| Run | Positional-compositional? | Receiver threshold | Rounds-to-crack | Trajectory (cp:acc) |
|---|---|---|---|---|
| 1 | no | 0.53 | — not cracked | 10:0.25 20:0.25 30:0.00 40:0.00 |
| 2 | no | 0.70 | — not cracked | 10:0.62 |
| 3 | yes | 0.73 | — not cracked | 10:0.12 20:0.00 |
| 4 | yes | 0.80 | — not cracked | 10:0.25 |
| 5 | no | 0.67 | — not cracked | 10:0.25 |

*Every probe (raw E reply included) is in the hash-chained result JSONL beside this file. The source campaign provenance is read-only and untouched.*
