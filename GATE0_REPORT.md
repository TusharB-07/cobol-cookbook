# GATE 0 — Baseline Audit Report

**Date:** 2026-09-21  
**Repo:** cobol-cookbook  
**Total tasks:** 25

| # | Program | Tier | .cbl File | test-input.txt | Compile | Run | Output Match | Status |
|---|---------|------|-----------|----------------|---------|-----|--------------|--------|
| 001 | bizzbuzz | 🥉 | bizzbuzz.cbl | MISSING | ✅ PASS | ✅ PASS | ❌ FAIL (leading zeros) | **RUNFAIL** |
| 002 | namebanner | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 003 | simple-interest | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 004 | celsius-fahrenheit | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 005 | reverse-string-manual | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 006 | vowel-counter | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 007 | largest-of-five | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 008 | multiplication-table | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 009 | sum-of-digits | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 010 | leap-year | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 011 | srm-foss-game | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 012 | star-pyramid | 🥉 | MISSING | MISSING | — | — | — | **MISSING** |
| 013 | student-grades | 🥈 | MISSING | MISSING | — | — | — | **MISSING** |
| 014 | phone-formatter | 🥈 | MISSING | MISSING | — | — | — | **MISSING** |
| 015 | word-count | 🥈 | MISSING | MISSING | — | — | — | **MISSING** |
| 016 | email-validator | 🥈 | MISSING | MISSING | — | — | — | **MISSING** |
| 017 | inventory-report | 🥈 | MISSING | MISSING | — | — | — | **MISSING** |
| 018 | temps-week | 🥈 | MISSING | MISSING | — | — | — | **MISSING** |
| 019 | palindrome | 🥈 | MISSING | MISSING | — | — | — | **MISSING** |
| 020 | currency-converter | 🥈 | MISSING | MISSING | — | — | — | **MISSING** |
| 021 | report-generator | 🥇 | MISSING | MISSING | — | — | — | **MISSING** |
| 022 | fizzbuzz-jcl | 🥇 | MISSING | MISSING | — | — | — | **MISSING** |
| 023 | cobol-vs-python | 🥇 | MISSING | MISSING | — | — | — | **MISSING** |
| 024 | expression-calculator | 🥇 | MISSING | MISSING | — | — | — | **MISSING** |
| 025 | caesar-cipher | 🥇 | MISSING | MISSING | — | — | — | **MISSING** |

## Summary
- **PASS:** 0
- **RUNFAIL:** 1 (001-bizzbuzz — leading zeros on numeric DISPLAY)
- **COMPILEFAIL:** 0
- **MISSING:** 24 (no .cbl files exist)

## Missing Files List
All 24 tasks (002–025) need:
1. Solution `.cbl` file in `programs/NNN-name/`
2. `test-input.txt` with stdin test data (per README specs)

## 001-bizzbuzz Detail
**Compile:** Warning only (missing newline at EOF)  
**Run Output:** Shows `01`, `02`, `04`... (leading zeros from `PIC 9(2)`)  
**Expected Output:** `1`, `2`, `4`... (no leading zeros)  
**Fix Needed:** Apply B1 convention — use `PIC Z9` or `FUNCTION TRIM` or edit-mask for displayed numbers