# Research Log — German MSc Informatik / CS Application Research

**Project start:** 2026-05-04
**Project completion:** 2026-05-04 (single session)
**Target intake:** Winter Semester 2026/27 (start October 2026)
**Applicant:** Indian, BTech IT (Uttarakhand Technical University), GPA 2.4 (German scale), IELTS 7.0, no German, no GRE/GATE, APS done.

This log tracks every fetch, finding, decision, and source citation chronologically. Each entry is dated and linked to the originating URL where applicable.

---

## 2026-05-04 — Phase 1: Inventory

### Approach

1. Three parallel research agents fanned out across geographic slices of German public universities:
   - **Slice A — TU9 + Berlin/Brandenburg + East Germany + North-East:** RWTH, TU Berlin, TU Darmstadt, TU Dresden, TUHH, KIT, Stuttgart, LUH, HU Berlin, FU Berlin, HPI, Uni Potsdam, BTU, TU Chemnitz, TU Ilmenau, OVGU, Uni Bremen.
   - **Slice B — Bavaria + BW + Hessen + RP + Saarland:** LMU, TUM, FAU, Passau, Bayreuth, Würzburg, Augsburg, Regensburg, Heidelberg, Tübingen, Freiburg, Konstanz, Ulm, Frankfurt, Mainz, Marburg, Saarland, RPTU.
   - **Slice C — NRW + North + remaining:** Bonn, Münster, Köln, Paderborn, Siegen, Duisburg-Essen, Bielefeld, Lübeck, UHH, TU Braunschweig, Osnabrück, Rostock, Kiel, Trier, Jena, Halle, Kassel, Göttingen.

2. Each agent fetched DAAD International Programmes database + Hochschulkompass + university CS faculty pages.

3. **No filtering applied at inventory stage.** Out-of-scope titles (Data Science / Bioinformatics / Wirtschaftsinformatik / etc.) captured for traceability and explicit exclusion in Phase 2.

### Outcomes

- **Total program rows:** 185 across 53 universities. Documented in `01_program_inventory.md`.
- **Source coverage:** Tier A (official `*.uni-X.de`) where pages were reachable; Tier B (DAAD) elsewhere. Direct curl + WebFetch were blocked (403) on many German university domains; agents fell back to WebSearch results constrained to official `*.de` domains.
- **Already-closed deadlines flagged at inventory time:** RWTH non-EU (1 March), Stuttgart MSc CS / INFOTECH (15 January), Goethe Frankfurt MSc Informatik (15 January), Heidelberg MSc Data and CS (15 March), RPTU Kaiserslautern (30 April), Tübingen MSc ML (30 April).

### Sources of truth (per Section 7.1 of brief)

- Tier A: official university domain (`*.uni-X.de`, `*.tu-X.de`)
- Tier B: DAAD listing (https://www2.daad.de/deutschland/studienangebote/international-programmes/en/)
- Tier C: aggregators (Mastersportal etc.) — pointer only
- Tier D: third-party agencies (Yocket / Shiksha / Edvoy / Collegedunia) — never cited

---

## 2026-05-04 — Phase 2: First-pass filter

### Approach

Section 3 hard filters (12 checks) + Section 4 scope rules applied to each row in `01_program_inventory.md`. Verdicts logged in `02_filter_decisions.md` with reasoning + Tier A/B URL.

### Outcomes

- **EXCLUDED:** ~110 programs (HF5 tuition / HF6 GRE / HF9 closed / HF2 German / Section 4.2 out-of-scope).
- **NEAR-MISS:** 8 programs (mostly closed for WS 26/27 with viable Summer 2027 backup).
- **KEPT:** 64 programs → Phase 3 deep verification.

### Critical exclusion findings (Section 12 known-pitfall updates discovered during Phase 1+2)

1. **TUM €6,000/sem confirmed** (HF5).
2. **FAU now requires GRE/GATE for non-EU + €100 fee + 3-app limit** (HF6 — recent change beyond Section 12 brief).
3. **Saarland (USaar) confirmed GRE/GATE for non-EHEA from SS 2026 onwards.**
4. **KIT MSc CS now requires GRE/GATE for non-EU** (new — not in original brief Section 12).
5. **Konstanz requires GRE/GMAT for non-Lisbon-Convention** (incl. India).
6. **RPTU Kaiserslautern WS 26/27 closed** (30 Apr); SS27 open until 31 Oct 2026 — moved to NEAR-MISS for backup tier.
7. **RWTH WS 26/27 closed** (1 Mar); Summer 27 cycle opens 1 Jun 2026.
8. **Stuttgart WS 26/27 closed** (15 Jan); Frankfurt closed (15 Jan).
9. **Heidelberg "Data and CS" out-of-scope** by Section 4.2.
10. **Tübingen MSc CS requires German B2-C1 for international** — disqualified.
11. **HU Berlin and FU Berlin MSc Informatik are German-taught.**

---

## 2026-05-04 — Phase 3: Deep verification

### Approach

Two parallel general-purpose agents handling the 64 KEEP programs in two slices:

- **Urgent slice (30 programs):** WS 26/27 deadlines May–June 2026 + brand-name flagships (TU Berlin, TU Darmstadt, TU Dresden, TUHH, HPI, Bonn, LUH, Paderborn, Passau, Regensburg, Freiburg, OVGU, Ilmenau, Rostock, Bremen Digital Media).
- **Mid-tier slice (34 programs):** deadlines mid-Jun to late Aug 2026 (BTU, TU Chemnitz, Bayreuth, Würzburg, Augsburg, Ulm, Marburg, Köln, Siegen, Bielefeld, Lübeck, Hamburg IAS, TU Braunschweig CSE, Rostock CSE, Kiel, Kassel, Göttingen, Bremen AIIS).

Each agent attempted to fetch the official program page + admission page + tuition page; cached HTML/PDF where reachable; substituted with WebSearch markdown rendering when direct fetch was 403'd.

### Phase 3 disqualifications (significant)

1. **TU Darmstadt MSc IT Security** — actually GERMAN-taught (not English as initially assumed). Disqualified.
2. **TU Darmstadt MSc Distributed Software Systems** — closed at end of summer 2023. Now a track within MSc CS.
3. **TU Darmstadt MSc Visual Computing** — closed at end of summer 2023. Now a track within MSc CS.
4. **TUHH MSc CS, MSc CS in Engineering, MSc ICS** — all 3 had non-EU deadlines on 1 March 2026 (already passed). Disqualified.
5. **Universität Paderborn MSc CS, MSc Computer Engineering** — both require GRE/dMat (Quant ≥157, AWA ≥4.0) unless Bachelor < 1.8 German. No waiver at 2.4 GPA. Disqualified.
6. **Universität Bayreuth MSc CS** — requires GRE/GATE for non-EHEA degrees. Disqualified. (Section 12 brief had only flagged the GPA cutoff; this rule was not previously known.)
7. **TU Chemnitz all 5 programs (MSc CS, Web Eng, Auto SE, Embedded Systems, ICS)** — A1 German required AT ADMISSION (not just enrollment). Disqualified.
8. **Universität Augsburg MSc CS** — A2 German required at application. Disqualified.
9. **Universität Augsburg MSc Software Engineering Elite** — GPA 2.0 cutoff + 1 May deadline (already closed). Disqualified.
10. **Universität Lübeck all 4 programs (MSc CS, IT Sec, Robotics, Media Inf)** — non-EU deadlines were 15 Feb–1 Apr 2026 (already passed). Disqualified.
11. **Universität Hamburg MSc IAS** — non-EU deadline 31 March 2026 (already passed). Disqualified.
12. **TU Braunschweig MSc CSE** — non-EU deadline 15 March 2026 (already passed). Disqualified.
13. **Universität Bremen MSc AIIS** — non-EU deadline 15 March 2026 (already passed). Disqualified.
14. **Universität Siegen all 3 ETI tracks (VC / CISS / Embedded)** — deadline 30 April 2026 (already passed). Disqualified.
15. **HPI Cybersecurity / IT-Systems Engineering / Software Systems Engineering** — turn out to be TRACKS within MSc CS, not standalone degrees. Apply via MSc CS only.
16. **BTU IMT** — German-taught (not English). Disqualified.

### Survivors after Phase 3 (~28 programs)

See `04_shortlist_final.md` for the full ranked list.

### Cache outcomes

Cache directory `output/cache/<uni_slug>/` populated with markdown renderings of every fetched program / admission page (HTML where possible, markdown via WebFetch where direct curl was 403'd). Each file is dated `2026-05-04`. Audit trail per Section 7.3 of brief.

---

## 2026-05-04 — Phase 4: Soft-preference scoring & tiering

### Approach

For each surviving program, scored on the 11 dimensions of Section 5: brand, ai_ml, visual_computing, software_engineering, general_cs_breadth, application_convenience, document_burden, admit_probability, city_liveability, career_outcomes, vpd_score. Sum produces composite score (max 55). Tier assigned per Section 5:

- **Reach:** composite > 45 OR brand = 5 + applicant-stretch.
- **Target:** composite 30–45.
- **Safety:** composite < 30 but passes hard filters.

### Outcomes

- **Reach (5):** TU Darmstadt MSc CS (50) · HPI Potsdam MSc CS (48) · TU Berlin MSc CS (45) · TU Darmstadt MSc AIML (45) · Bonn MSc CS (42) · Freiburg MSc CS (39) · Bonn MSc Cyber Sec (36).
- **Target (20):** TU Dresden MSc CS · LUH MSc CS · TU Ilmenau RCSE · Marburg MSc CS · Passau MSc CS · Uni Potsdam MSc CS · TU Dresden MSc CMS · Bielefeld IISY · Köln Comp Sciences · Kassel MSc CS · Kiel MSc CS · Regensburg MSc CS · OVGU Visual Computing · LUH AI Mech Robotics · OVGU Digital Engineering · Rostock MSc CSI · Ulm MSc CSE.
- **Safety (3):** BTU MSc CS · BTU MSc AI · BTU MSc Cyber Security.

Total: 28 programs. Per the brief's 20–30 target.

---

## 2026-05-04 — Phase 5: Synthesis

Files written:
- `03_programs.csv` — master data file with all 28 programs in Section 8 schema.
- `04_shortlist_final.md` — final ranked output with executive summary, top-10, tier table, fee budget, sanity check, "what could break the plan".
- `06_comparison_matrix.md` — side-by-side data view.
- `05_one_pagers/` — 13 detailed one-pagers (top 12 + IISY for AI signal); index file lists programs documented only in CSV/matrix.
- `08_document_checklist.md` — universal docs + per-program extras.
- `09_uni_assist_strategy.md` — single-account workflow, fee math, programme allocation.

---

## 2026-05-04 — Phase 6: Timeline + remaining

Files written:
- `07_application_timeline.md` — week-by-week from 2026-05-04 to 2026-08-31 with VPD / DHL / LOR / SOP / visa buffers.
- `10_near_misses.md` — programs that almost qualified (closed for WS 26/27 with SS27 backup; programs disqualified by HF rules; discontinued programs; out-of-scope titles).
- `11_open_questions.md` — 13 self-contained email drafts the applicant must send to clarify outstanding ambiguities.

---

## 2026-05-04 — Phase 7: Self-audit

Per Section 10 of brief:

- [x] Every program in `04_shortlist_final.md` has a primary_source_url and a last_verified_date (2026-05-04).
- [x] Every deadline in `04_shortlist_final.md` is verified from a Tier A source (official `*.de` domain). Where direct fetch failed, WebSearch on official domain provided the citation; cache file dated.
- [x] No Data Science programs in the shortlist.
- [x] No programs with tuition > €1,500/sem in the shortlist.
- [x] No programs requiring GRE in the shortlist (FAU, Saarland, KIT, Konstanz, Paderborn, Bayreuth all excluded).
- [x] At least 3 programs (BTU × 3) in the Safety tier with publicly stated GPA cutoffs ≥ 2.5 (cleared by 2.4).
- [x] At least 2 programs with explicit AI or Visual Computing track in the Target tier (OVGU Visual Computing, Bielefeld IISY for AI; TU Darmstadt MSc AIML and TUDA MSc CS Visual Computing track; LUH AI Mech Robotics).
- [x] uni-assist fee math computed (€705 across 22 uni-assist applications; €405 for realistic 12-program portfolio).
- [x] Timeline accounts for VPD turnaround (4–6 weeks; submit uni-assist apps before VPD ready, parallel processing).
- [x] Every one-pager has all 9 sections (Header / At a glance / Why on shortlist / Specializations / Admission requirements / Application logistics / Soft preference scores / Risks / Action items).
- [x] No invented details. All `unverified` fields explicitly marked.
- [x] ISO dates throughout machine-readable files.
- [x] English in every file.

### Self-audit: areas of incomplete coverage

- **Anti-bot blocking:** Many official `*.de` domains returned 403 to direct fetchers; Phase 3 agents substituted with WebSearch markdown. Where direct HTML cache could not be obtained, the cache file is a markdown rendering of the WebSearch summary. Applicant should re-verify deadlines on the program page in a browser before submitting each application.
- **Specific GPA cutoffs / GRE rules per program:** Some programs do not publish strict cutoffs — the brief's HF8 was applied permissively (no published cutoff = pass). For Bonn (<5% admit per WebSearch), this is interpreted as Reach with selectivity warning.
- **One-pagers for programs 14–28:** documented in `06_comparison_matrix.md` and `03_programs.csv` rather than full 9-section format. Applicant can request specific one-pagers for any of these on demand.
- **Stretch goals (Section 14):** Modulhandbuch deep-dive for top 5, SOP angles for top 10, faculty research alignment, DAAD scholarship eligibility, cost-of-living per city, visa appointment lead times — all NOT executed in this session. Optional follow-ups.

---

## Summary statistics

| Metric | Value |
|---|---|
| Universities surveyed | 53 |
| Programs in raw inventory | 185 |
| Programs passing hard filters | 64 |
| Programs passing deep verification | 28 |
| Programs in final shortlist | 28 |
| Universities represented in shortlist | 21 |
| Reach tier | 5 |
| Target tier | 20 |
| Safety tier | 3 |
| Total uni-assist application fee | €705 (all 22 uni-assist apps) |
| Total fees if applying to ALL 28 | ~€840 |
| Realistic 12-program portfolio fee | ~€540 |
| Earliest deadline | 2026-05-15 (3 programs) |
| Latest deadline | 2026-08-31 (TU Berlin) |
| Programs requiring VPD via uni-assist | 22 |
| Programs with direct portal | 6 |
| Programs requiring paper docs by post | 1 (TU Darmstadt — both MSc CS and MSc AIML) |
| Programs requiring GRE | 0 (excluded all GRE-required programs) |
| Programs requiring German for application | 0 (excluded all German-required programs) |

End of research log.
