# PHASE 0 — Audit Table

| File | Compile | Run | Notes |
|------|---------|-----|-------|
| programs/001-bizzbuzz/bizzbuzz.cbl | PASS | RUNFAIL | Zero-padding: outputs `01`, `02` vs expected `1`, `2` |
| programs/900-t-good/good.cbl | PASS | PASS | Torture test - known good |
| programs/901-t-broken/broken.cbl | FAIL | — | Torture test - syntax error |
| programs/902-t-stdin/stdin.cbl | PASS | PASS | Torture test - reads stdin |
| programs/903-t-loop/loop.cbl | PASS | FAIL | Torture test - infinite loop (timeout kills) |
| programs/002-namebanner/*.cbl | MISSING | — | No .cbl file |
| programs/003-simple-interest/*.cbl | MISSING | — | No .cbl file |
| programs/004-celsius-fahrenheit/*.cbl | MISSING | — | No .cbl file |
| programs/005-reverse-string-manual/*.cbl | MISSING | — | No .cbl file |
| programs/006-vowel-counter/*.cbl | MISSING | — | No .cbl file |
| programs/007-largest-of-five/*.cbl | MISSING | — | No .cbl file |
| programs/008-multiplication-table/*.cbl | MISSING | — | No .cbl file |
| programs/009-sum-of-digits/*.cbl | MISSING | — | No .cbl file |
| programs/010-leap-year/*.cbl | MISSING | — | No .cbl file |
| programs/011-srm-foss-game/*.cbl | MISSING | — | No .cbl file |
| programs/012-star-pyramid/*.cbl | MISSING | — | No .cbl file |
| programs/013-student-grades/*.cbl | MISSING | — | No .cbl file |
| programs/014-phone-formatter/*.cbl | MISSING | — | No .cbl file |
| programs/015-word-count/*.cbl | MISSING | — | No .cbl file |
| programs/016-email-validator/*.cbl | MISSING | — | No .cbl file |
| programs/017-inventory-report/*.cbl | MISSING | — | No .cbl file |
| programs/018-temps-week/*.cbl | MISSING | — | No .cbl file |
| programs/019-palindrome/*.cbl | MISSING | — | No .cbl file |
| programs/020-currency-converter/*.cbl | MISSING | — | No .cbl file |
| programs/021-report-generator/*.cbl | MISSING | — | No .cbl file |
| programs/022-fizzbuzz-jcl/*.cbl | MISSING | — | No .cbl file |
| programs/023-cobol-vs-python/*.cbl | MISSING | — | No .cbl file |
| programs/024-expression-calculator/*.cbl | MISSING | — | No .cbl file |
| programs/025-caesar-cipher/*.cbl | MISSING | — | No .cbl file |

**Summary:** 1 real program (RUNFAIL - zero padding), 4 torture tests, 24 missing