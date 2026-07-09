# Review Status

## Fixed

| Issue | Status |
|---|---|
| ProcessOperation wrong algorithm number (was hardcoded "9") | Fixed — now uses `\ref{alg:process-operation}` |
| Operations Verifiability undefined | Fixed — formal game + advantage definition + theorem now in §7 |
| Overly-tailored signature/AEAD definitions | Fixed — moved into `\iffalse` block (effectively removed) |
| NARK formal definition missing | Fixed — `Definition[NARK]` added to §3 |
| Theorems had no advantage notation | Fixed — FS and PCS theorems now have proper Adv terms |

## Partially Fixed

| Issue | What's There | What's Still Missing |
|---|---|---|
| FS/PCS security proofs | Theorems exist with sketched reductions | No formal game definitions for FS or PCS — IND-CCA is referenced but never defined in the paper |
| Anonymous credentials | Properties listed (unlinkability, revocability, expiry) | No formal security definitions, no proofs |
| Bulletproofs statements | $\mathcal{R}_{\text{sat}}$ formally defined | Relations inside the circuits still described informally |
| Malicious insider model | Formal game + definition added | Still no explicit adversary capability list (concurrent ops, delays, stale states) |

## Not Fixed

| Issue | Where |
|---|---|
| MLS adoption mischaracterized — still says "not yet widely adopted," only mentions Wire. Google Meet, Discord, Webex, RCS are absent | `1-introduction.tex:12`, `2-related-work.tex:9` |
| "Removing the signature" for anonymity — still unexplained and unclear | `6-zk-rbac.tex:2` |
| "Users not explicitly identified" — reviewer called this confusing; still in the text | `7-security.tex:7` |
| X3DH still a static function — no protocol formalism | `3-preliminaries.tex:41` |
| ART undefined in abstract — "constructions (such as ART)" with no expansion | `0-abstract.tex:1` |
| Why ART over TreeKEM? — never directly answered | Introduction, Related Work |
| Anonymous eligibility motivation — "anonymity from whom?" never answered | `6-zk-rbac.tex` |
