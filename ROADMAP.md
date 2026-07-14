# Okie Original Grow Tracker — Build Roadmap

This file is the running game plan. Check items off as they're finished.
Update this file (and commit it) at the end of every work session, even if only one box got checked.

---

## Phase 0 — Foundation
- [x] GitHub repo created under okie-original org (`grow-tracker`)
- [x] GitHub Pages turned on, live at `okie-original.github.io/grow-tracker/`
- [x] Binding ToS / private-property agreement gate built and working (one-time per device)
- [x] Old Supabase project wiped, fresh empty project ready
- [x] GitHub repo wiped clean, starting from scratch

## Phase 1 — Database Schema
- [ ] Design `strains` table (name, parents/lineage links, notes)
- [ ] Design `seeds` table (strain link, count, fem/regular, low-stock thresholds)
- [ ] Design `plants` table (strain link, stage, tent link, activity log)
- [ ] Design `tents` table
- [ ] Design `crosses` / breeding table (mom, dad, resulting seed batch, phenotype notes)
- [ ] Build these tables in the new Supabase project
- [ ] Test basic read/write from a scratch HTML page to confirm connection works

## Phase 2 — Seed Vault App
- [ ] Basic list view of strains/seed stock
- [ ] Color-coded low-stock indicators (green/yellow/red)
- [ ] "Pull seeds" flow — enter quantity, auto-deduct from stock
- [ ] Empty seed lines move out of sight instead of deleting (so a line can be reused for F2s etc.)
- [ ] Parent strain fields as real linked records, not plain text (e.g. splitting "H.S.B. x I.C.C." into linked strains)
- [ ] Import existing seed stock data from the old InfinityFree JSON export

## Phase 3 — Plants / Tents App
- [ ] Plant list with stage tracking
- [ ] Tent grouping
- [ ] Bulk actions (e.g. water whole tent with one tap)
- [ ] Per-plant activity log
- [ ] Import existing plant data from the old InfinityFree JSON export

## Phase 4 — Breeding App
- [ ] Cross records (mom x dad -> resulting seeds)
- [ ] Phenotype tracking per cross (not just visual, but effect/quality notes)
- [ ] Family tree / lineage view, forward and backward
- [ ] Bank tracking for F8-ish plants crossed back to the same male

## Phase 5 — Hub Landing Page
- [ ] Single landing page linking Seed Vault, Plants/Tents, and Breeding
- [ ] Sits behind the same ToS gate
- [ ] Matches dark/orange Okie Original theme

## Phase 6 — Later / Nice-to-Have
- [ ] Photo capture that auto-links to a tracker entry
- [ ] AI-generated notes from photos
- [ ] AI-assisted lineage guessing from leaf traits

---

## Changelog
- 2026-07-14: Foundation phase completed — repo, Pages hosting, ToS gate, fresh Supabase project.
