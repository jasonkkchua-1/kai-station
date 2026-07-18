# 解 kai — lexicon audit (injectivity vs. the positional rule)

*Offline recomputation from campaign provenance (READ ONLY). Modal lexicon = most frequent word per training object over the last 40 rounds.*

The campaign's `compositional` flag applies a POSITIONAL-CONSISTENCY rule: one symbol position tracks colour and the other tracks shape. That rule does **not** require INJECTIVITY. A run can pass positional consistency while assigning the same word to two different objects (a HOMONYM). A CLEAN compositional code is both positional and injective (a genuine one-to-one grammar).

## C1 — `kumi-provenance.jsonl`

| Run | n | Modal lexicon (obj:word) | Positional? | Homonym (word→objs) | CLEAN (injective)? |
|---|---|---|---|---|---|
| 1 | 49 | 1:●●, 2:▲▲, 3:●■ | no | — | no |
| 2 | 23 | 1:●■, 2:■●, 3:●■ | no | ●■→[1, 3] | no |
| 3 | 33 | 1:■●, 2:■■, 3:●● | yes | — | YES |
| 4 | 20 | 1:▲●, 2:▲■, 3:■● | yes | — | YES |
| 5 | 21 | 1:●▲, 2:■●, 3:●■ | no | — | no |

**C1 counts** — positional-compositional: 2/5 · CLEAN (injective) compositional: **2/5** · campaign CLAIMED: 2/5.

## C2 — `kumi2-provenance.jsonl`

| Run | n | Modal lexicon (obj:word) | Positional? | Homonym (word→objs) | CLEAN (injective)? |
|---|---|---|---|---|---|
| 1 | 21 | 1:▲■, 2:▲●, 3:▲■ | yes | ▲■→[1, 3] | no |
| 2 | 120 | 1:▲●, 2:▲■, 3:▲● | yes | ▲●→[1, 3] | no |
| 3 | 48 | 1:▲●, 2:▲●, 3:▲■ | yes | ▲●→[1, 2] | no |
| 4 | 81 | 1:▲■, 2:▲●, 3:▲■ | yes | ▲■→[1, 3] | no |
| 5 | 36 | 1:▲●, 2:▲■, 3:■● | yes | — | YES |

**C2 counts** — positional-compositional: 5/5 · CLEAN (injective) compositional: **1/5** · campaign CLAIMED: 5/5.
> The claimed 5/5 counts positionally-consistent runs; only 1/5 are injective. The difference is homonymous codes (two objects, one word).

*Audit is arithmetic on read-only provenance; no model was queried. Kai measures observability only.*
