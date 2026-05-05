# Filter Decisions — Per-Program Kept / Excluded Reasoning

**Date built:** 2026-05-04
**Input:** `01_program_inventory.md` (185 program rows)
**Method:** Apply Section 3 hard filters (12 checks) + Section 4 scope rules to each row. Record verdict + primary reason + Tier A/B URL.
**Today is 2026-05-04** — programs with WS 26/27 deadline before this date are flagged "WS 26/27 closed"; if a Summer 2027 alternative exists, the program may be retained as a backup-tier candidate.

---

## Hard filter codes

- **HF1** — CS-discipline degree (Section 4.1)
- **HF2** — English-taught (full program or English track)
- **HF3** — IELTS requirement ≤ 7.0 (applicant has IELTS 7.0)
- **HF4** — No German required for application or first-semester compulsory modules
- **HF5** — Tuition ≤ €1,500/sem
- **HF6** — No GRE/GATE required
- **HF7** — Indian 4-year BTech IT accepted (with APS) — assumed yes if not stated otherwise
- **HF8** — GPA cutoff ≤ 2.5 German scale (applicant 2.4)
- **HF9** — WS 26/27 application open (deadline ≥ 2026-05-05)
- **HF10** — Public university
- **HF11** — Standalone consecutive MSc (120 ECTS / 4 sem)
- **HF12** — APS-eligible

## Verdict codes

- **KEEP** — passes all hard filters and is in scope. Goes to Phase 3 deep verification.
- **EXCLUDE** — fails one or more hard filters or is Section 4.2 out-of-scope.
- **NEAR-MISS** — borderline; goes to `10_near_misses.md` for applicant review (e.g. closed for WS 26/27 but open for SS27, or specialisation worth flagging).

---

## EXCLUSIONS — Section 3 hard-filter failures

### TUM (5 programs) — fail HF5 (€6,000/sem)

All TUM CIT/Informatik programs charge €6,000/sem for non-EU students. Disqualified by Section 3 hard filter 5.

| # | Program | Reason | URL |
|---|---|---|---|
| 80 | TUM M.Sc. Informatics | HF5 fail — €6,000/sem non-EU | https://www.cit.tum.de/en/cit/studies/degree-programs/master-informatics/ |
| 81 | TUM M.Sc. Data Engineering and Analytics | HF5 fail + Section 4.2 (Data) | https://www.cit.tum.de/en/cit/studies/degree-programs/ |
| 82 | TUM M.Sc. Robotics, Cognition, Intelligence | HF5 fail | https://www.in.tum.de/en/for-prospective-students/masters-programs/robotics-cognition-intelligence-msc/ |
| 83 | TUM M.Sc. Computational Science and Engineering | HF5 fail | https://www.tum.de/en/studies/degree-programs/detail/computational-science-and-engineering-cse-master-of-science-msc |
| 84 | TUM M.Sc. Bioinformatics (joint LMU+TUM) | HF5 fail + Section 4.2 (Bio) | https://www.tum.de/en/studies/degree-programs/detail/bioinformatics-master-of-science-msc-1 |

### FAU Erlangen-Nürnberg (5 in-scope CS programs) — fail HF6 (GRE/GATE)

FAU has introduced a GRE/GATE >60th percentile requirement for non-EU applicants starting WS 26/27, plus a €100 non-EU application fee and a 3-application cap per applicant. Disqualified by Section 3 hard filter 6.

| # | Program | Reason | URL |
|---|---|---|---|
| 85 | FAU M.Sc. Artificial Intelligence | HF6 fail — GRE/GATE required (new WS 26/27) | https://www.fau.eu/degree-program/artificial-intelligence-ai-m-sc/ |
| 87 | FAU M.Sc. Computational Engineering | HF6 fail | https://www.fau.eu/degree-program/computational-engineering-ce-m-sc |
| 88 | FAU M.Sc. Information and Communication Technology | HF6 fail | https://www.fau.eu/degree-program/information-and-communication-technology-iuk-m-sc/ |
| 89 | FAU M.Sc. Communications and Multimedia Engineering | HF6 fail | https://www.fau.eu/degree-program/communications-and-multimedia-engineering-m-sc/ |
| 90 | FAU M.Sc. Advanced Signal Processing & Communications Engineering (ASC) | HF6 fail | https://www.asc.studium.fau.de/ |

### Universität des Saarlandes (8 CS-discipline programs) — fail HF6

USaar (Saarland Informatics Campus) requires GRE General OR Indian GATE for all non-EHEA applicants from SS 2026 onwards. Section 12 pitfall confirmed.

| # | Program | Reason | URL |
|---|---|---|---|
| 125 | USaar M.Sc. Computer Science | HF6 fail | https://www.uni-saarland.de/en/study/programmes/master/informatics.html |
| 126 | USaar M.Sc. Cybersecurity | HF6 fail | https://saarland-informatics-campus.de/en/studium-studies/master-english/faq-cyber-application/ |
| 127 | USaar M.Sc. Entrepreneurial Cybersecurity | HF6 fail (assumed same rule) | https://cysec.uni-saarland.de/master/ecs/ |
| 129 | USaar M.Sc. Embedded Systems | HF6 fail | https://www.uni-saarland.de/en/study/programmes/master/embedded-systems.html |
| 130 | USaar M.Sc. Visual Computing | HF6 fail | https://saarland-informatics-campus.de/en/msc-visual-computing/ |
| 132 | USaar M.Sc. Media Informatics | HF6 fail | https://www.uni-saarland.de/en/study/programmes/master/media-informatics.html |
| 135 | USaar M.Sc. Mathematics and Computer Science | HF6 fail (verify in Phase 3) | https://saarland-informatics-campus.de/en/studium-studies/master-english/ |
| 128 | USaar M.Sc. Data Science and AI | HF6 fail + Section 4.2 (Data) | https://saarland-informatics-campus.de/en/studium-studies/data-science-and-artificial-intelligence-master/ |

### KIT — fail HF6

KIT MSc Computer Science requires GRE/GATE for non-EU applicants.

| # | Program | Reason | URL |
|---|---|---|---|
| 27 | KIT M.Sc. Computer Science | HF6 fail (GRE/GATE required for non-EU) | https://www.sle.kit.edu/english/vorstudium/master-computer-science.php |

### Universität Konstanz — fail HF6

Konstanz MSc Computer and Information Science requires GRE/GMAT for applicants from non-Lisbon-Convention countries (including India).

| # | Program | Reason | URL |
|---|---|---|---|
| 115 | Uni Konstanz M.Sc. Computer and Information Science | HF6 fail (GRE/GMAT required for India) + 15 Apr CLOSED for visa | https://www.uni-konstanz.de/en/study/before-you-study/study-programmes/detail/computer-and-information-science/ |

### RWTH Aachen — fail HF9 (closed) + HF6 (GRE for non-EU)

RWTH non-EU deadline of 1 March 2026 has passed for WS 26/27. Additionally, GRE is required for non-EU applicants. Summer 2027 application window opens 1 June 2026 — flag as NEAR-MISS for backup tier.

| # | Program | Reason | URL |
|---|---|---|---|
| 1 | RWTH M.Sc. Computer Science | HF9 fail (1 Mar CLOSED) + HF6 fail | https://www.informatik.rwth-aachen.de/cms/informatik/studium/vor-dem-studium/~nhhb/masterstudiengaenge/?lidx=1 |
| 2 | RWTH M.Sc. Software Systems Engineering | HF9 + HF6 fail | https://www.rwth-aachen.de/cms/root/studium/vor-dem-studium/studiengaenge/liste-aktuelle-studiengaenge/studiengangbeschreibung/~bnhr/software-systems-engineering-m-sc/?lidx=1 |
| 3 | RWTH M.Sc. Media Informatics | HF9 likely + verify status (possibly discontinued) | https://www.b-it-center.de/b-it-programmes/msc-in-media-informatics/description |
| 4 | RWTH M.Sc. Human-Centered Intelligent Systems | HF9 likely + HF6 likely | https://www.rwth-aachen.de/cms/root/studium/vor-dem-studium/studiengaenge/liste-aktuelle-studiengaenge/studiengangbeschreibung/~bltdwv/human-centered-intelligent-systems-m-sc/?lidx=1 |
| 5 | RWTH M.Sc. Computer Engineering | HF9 likely + HF6 likely | https://www.rwth-aachen.de/cms/root/studium/vor-dem-studium/studiengaenge/liste-aktuelle-studiengaenge/studiengangbeschreibung/Computer-Engineering-M-Sc/?lidx=1 |
| 7 | RWTH M.Sc. Robotic Systems Engineering | HF5 fail (continuing-ed paid) | https://www.academy.rwth-aachen.de/en/programs/masters-degree-programs/detail/msc-robotic-systems-engineering |

### RPTU Kaiserslautern — fail HF9 for WS 26/27 (NEAR-MISS — SS27 open)

RPTU WS 26/27 deadline 30 April 2026 has passed. SS 2027 deadline is 31 October 2026 — viable backup. Move to NEAR-MISS for backup-tier review.

| # | Program | Reason | URL |
|---|---|---|---|
| 136 | RPTU M.Sc. Computer Science | HF9 fail (WS); SS27 open until 31 Oct 2026 → NEAR-MISS | https://applymsc.informatik.uni-kl.de/ |
| 137 | RPTU M.Sc. Embedded Computing Systems | HF9 fail (WS likely) | https://eit.rptu.de/en/esy/program-1 |
| 138 | RPTU M.Sc. Automation & Control | unverified | https://rptu.de/en/international/master/prospective-students/master-programs/master-programs-in-english |
| 139 | RPTU M.Sc. Software Eng for Embedded Systems | HF5 fail (Fernstudium tuition) | https://fernstudium.rptu.de/en/distance-learning-programmes/technology-engineering-and-natural-sciences/software-engineering-for-embedded-systems |

### Universität Stuttgart — fail HF9 for WS 26/27

Stuttgart MSc CS and INFOTECH WS 26/27 deadlines (15 January) have passed.

| # | Program | Reason | URL |
|---|---|---|---|
| 30 | Uni Stuttgart M.Sc. Computer Science | HF9 fail (15 Jan CLOSED) | https://www.uni-stuttgart.de/en/study/study-programs/Computer-Science-M.Sc.-00001/ |
| 31 | Uni Stuttgart M.Sc. INFOTECH | HF9 fail (15 Jan CLOSED) | https://www.infotech.uni-stuttgart.de/ |

### Goethe Frankfurt — fail HF9

Goethe Frankfurt MSc Informatik foreign-degree deadline 15 January 2026 has passed.

| # | Program | Reason | URL |
|---|---|---|---|
| 118 | Goethe Frankfurt M.Sc. Informatik | HF9 fail (15 Jan CLOSED) | https://www.uni-frankfurt.de/35791857/Informatik__Master_of_Science |

### Heidelberg — fail HF9 + Section 4.2

| # | Program | Reason | URL |
|---|---|---|---|
| 105 | Uni Heidelberg M.Sc. Data and Computer Science | Section 4.2 (Data in title) + HF9 fail (15 Mar CLOSED) | https://www.uni-heidelberg.de/en/study/all-subjects/computer-science/data-and-computer-science-master |
| 106 | Uni Heidelberg M.Sc. Scientific Computing | HF9 ambiguous (15 Mar CLOSED, 30 Sep alternate) — verify in Phase 3 | https://www.uni-heidelberg.de/en/study/all-subjects/scientific-computing/scientific-computing-master |

### Tübingen — multiple failures

| # | Program | Reason | URL |
|---|---|---|---|
| 108 | Uni Tübingen M.Sc. Computer Science | HF4 fail (German B2-C1 required for international applicants) | https://uni-tuebingen.de/en/study/finding-a-course/degree-programs-available/detail/course/computer-science-master/ |
| 109 | Uni Tübingen M.Sc. Machine Learning | HF8 fail (2.0 cutoff) + HF9 fail (30 Apr CLOSED) | https://uni-tuebingen.de/en/study/finding-a-course/degree-programs-available/detail/course/machine-learning-master/ |

### Universität Duisburg-Essen — fail HF4

| # | Program | Reason | URL |
|---|---|---|---|
| 155 | UDE M.Sc. Computer Engineering (ISE) | HF4 fail (German B2 required at enrollment) | https://www.uni-due.de/iw/en/study/m-ce.php |
| 156 | UDE M.Sc. Applied Computer Science | HF2 fail (German-taught primarily) | https://www.uni-due.de/computer-science/study-courses |

### TU Berlin Computer Engineering / Computational Neuroscience — fail HF2 / Section 4.2

| # | Program | Reason | URL |
|---|---|---|---|
| 9 | TU Berlin M.Sc. Computer Engineering | HF2 fail (mostly German) | https://www.tu.berlin/en/studying/study-programs/all-programs-offered/study-course/computer-engineering-m-sc |
| 11 | TU Berlin M.Sc. Computational Neuroscience | Section 4.2 (Cognitive/Neuro) | https://www.tu.berlin/en/studying/study-programs/all-programs-offered/study-course/computational-neuroscience-m-sc |

### TU Berlin ICT Innovation — borderline

| # | Program | Reason | URL |
|---|---|---|---|
| 10 | TU Berlin M.Sc. ICT Innovation | NEAR-MISS — EIT Digital double-degree, Erasmus Mundus structure (Section 4.1 allows EM); separate application process; flag for applicant | https://www.tu.berlin/studieren/studienangebot/gesamtes-studienangebot/studiengang/ict-innovation-m-sc |

### HU Berlin — fail HF2 / Section 4.2

| # | Program | Reason | URL |
|---|---|---|---|
| 36 | HU Berlin M.Sc. Computer Science | HF2 fail (primarily German, C1 German required) | https://www.hu-berlin.de/en/studies/counselling/course-catalogue/programme-descriptions/infmono |
| 37 | HU Berlin M.Sc. Information Systems | Section 4.2 (business IS) | https://www.wiwi.hu-berlin.de/en/Professorships/bwl/wi/master_information_system/master_is_en |
| 38 | HU Berlin M.Sc. Computational Neuroscience | Section 4.2 (Cog/Neuro) | https://www.bccn-berlin.de/master-program-application.html |

### FU Berlin — fail HF2 + Section 4.2

| # | Program | Reason | URL |
|---|---|---|---|
| 39 | FU Berlin M.Sc. Computer Science | HF2 fail (DSH German required) | https://www.fu-berlin.de/en/studium/studienangebot/master/informatik/index.html |
| 40 | FU Berlin M.Sc. Data Science | Section 4.2 (Data) | https://www.fu-berlin.de/en/studium/studienangebot/master/data-science/index.html |
| 41 | FU Berlin M.Sc. Bioinformatics | Section 4.2 (Bio) | https://www.mi.fu-berlin.de/en/bioinf/stud/studieninteressierte/index.html |
| 42 | FU Berlin M.Sc. Computational Sciences | unverified language — verify in Phase 3 | https://www.fu-berlin.de/en/studium/studienangebot/master/ |

### Other German-only Informatik MSc — fail HF2

| # | Program | Reason | URL |
|---|---|---|---|
| 13 | TU Darmstadt M.Sc. Informatik | HF2 fail (German) — but English MSc CS variant kept | https://www.informatik.tu-darmstadt.de/studium_fb20/im_studium/studiengaenge_liste/informatik_msc.en.jsp |
| 28 | KIT M.Sc. Informatics | HF2 fail (German) — and English MSc CS already excluded by GRE | https://www.sle.kit.edu/english/vorstudium/master-informatics.php |
| 29 | KIT M.Sc. Electrical Eng & IT | HF2 fail (mostly German) | https://www.sle.kit.edu/english/vorstudium/master-electrical-engineering-information-technology.php |
| 61 | TU Ilmenau M.Sc. Computer Science | HF2 fail (German primary) | https://www.tu-ilmenau.de/en/study/before-the-study/range-of-courses/master/computer-science-msc |
| 66 | OVGU M.Sc. Computer Science (Informatik) | HF2 fail (German primary) | https://www.ovgu.de/unimagdeburg/en/Study/Study+Programmes/Master/Computer+Science-p-17637.html |
| 76 | LMU München M.Sc. Informatik | HF2 fail (German + English electives only) | https://www.ifi.lmu.de/studium/studiengaenge/master/master_informatik/bewerbung/ |
| 92 | FAU M.Sc. Informatik | HF2 fail (German) — also FAU GRE rule | https://www.fau.eu/degree-program/informatik-m-sc |
| 97 | Uni Bayreuth M.Sc. Applied Computer Science | HF2 fail (German) — but English MSc CS kept | https://www.uni-bayreuth.de/en/master/applied-computer-science |
| 98 | Uni Bayreuth M.Sc. Informatik (German) | HF2 fail (German) | https://www.uni-bayreuth.de/en/master/computer-science-german |
| 119 | Uni Mainz M.Sc. Informatik | HF2 fail (DSH-2 / German C1 required for intl) | https://www.studies.fb08.uni-mainz.de/computer-science/prospective-students/master-of-science-computer-science/ |
| 120 | Uni Mainz M.Sc. Computer Science and Natural Sciences | HF2 fail (German) | https://www.studium.uni-mainz.de/en/choosing-your-degree-program/courses-offered/computer-and-natural-sciences-msc/ |
| 145 | Uni Münster M.Sc. Informatik | HF2 fail (German DSH-2) | https://www.uni-muenster.de/Informatik/en/ |
| 167 | Uni Hamburg M.Sc. Informatik | HF2 fail (German primary) | https://www.inf.uni-hamburg.de/en/studies/master/inf.html |
| 170 | TU Braunschweig M.Sc. Informatik | HF2 fail (German DSH 1+) | https://www.tu-braunschweig.de/en/degree-programmes/computer-science-master |
| 179 | Uni Trier M.Sc. Informatik | HF2 fail (German) | https://www.uni-trier.de/en/university/faculties-and-departments/faculty-iv/study-courses/computer-science/ |
| 180 | Uni Jena M.Sc. Computer Science | HF2 fail (German DSH-2) | https://www.uni-jena.de/en/6680/m-sc-computer-science |
| 181 | Uni Jena M.Sc. Computational and Data Science | HF2 fail (DSH-2 required) + Section 4.2 (Data) | https://www.uni-jena.de/en/6630/m-sc-computational-and-data-science |
| 182 | MLU Halle M.Sc. Informatik | HF2 fail (German) | https://studienangebot.uni-halle.de/informatik-master-120 |

### Out-of-scope titles — Section 4.2 exclusions

#### Data Science / Big Data / Data Engineering / Data Analytics

| # | Program | Reason | URL |
|---|---|---|---|
| 6 | RWTH M.Sc. Data Science | Section 4.2 (Data) | https://www.informatik.rwth-aachen.de/cms/informatik/studium/vor-dem-studium/~nhhb/masterstudiengaenge/?lidx=1 |
| 45 | HPI M.Sc. Data Engineering | Section 4.2 (Data Engineering) — phasing out | https://hpi.de/en/studies/before-your-studies/degree-programs/master.html |
| 64 | OVGU M.Sc. Data and Knowledge Engineering | Section 4.2 (Data direction) | https://www.ovgu.de/unimagdeburg/en/Study/Study+Programmes/Master/Data+and+Knowledge+Engineering-p-17625.html |
| 86 | FAU M.Sc. Data Science | Section 4.2 (Data) + HF6 | https://www.fau.eu/degree-program/data-science-m-sc/ |
| 124 | Uni Marburg M.Sc. Data Science | Section 4.2 (Data) | https://www.uni-marburg.de/en/studying/after-your-first-degree/masters-programs/degree-programs/data-science-msc |
| 158 | Uni Bielefeld M.Sc. Data Science | Section 4.2 (Data) | https://www.uni-bielefeld.de/fakultaeten/wirtschaftswissenschaften/studium-und-lehre/studiengaenge/master_data_science/ |
| 166 | Uni Hamburg M.Sc. Data Science and AI | Section 4.2 (Data) | https://www.inf.uni-hamburg.de/en/studies/master/dsai.html |
| 171 | TU Braunschweig M.Sc. Data Science | Section 4.2 (Data) | https://www.tu-braunschweig.de/en/degree-programmes |
| 177 | Uni Trier M.Sc. Data Science | Section 4.2 (Data) | https://www.uni-trier.de/en/studium/studienangebot/studiengaenge-von-a-z/english-taught-masters-courses-1 |

#### Bioinformatics / Medical Informatics / Life Science Informatics

| # | Program | Reason | URL |
|---|---|---|---|
| 78 | LMU+TUM M.Sc. Bioinformatics | Section 4.2 (Bio) | https://www.tum.de/en/studies/degree-programs/detail/bioinformatics-master-of-science-msc-1 |
| 110 | Uni Tübingen M.Sc. Bioinformatics | Section 4.2 (Bio) | https://uni-tuebingen.de/en/study/finding-a-course/degree-programs-available/detail/course/bioinformatics-master/ |
| 111 | Uni Tübingen M.Sc. Medical Informatics | Section 4.2 (Med Inf) | https://uni-tuebingen.de/en/study/finding-a-course/degree-programs-available/detail/course/medical-informatics-master/ |
| 122 | Uni Mainz M.Sc. Applied Bioinformatics | Section 4.2 (Bio) | https://www.studying.uni-mainz.de/applied-bioinformatics-m-sc/ |
| 131 | USaar M.Sc. Bioinformatics | Section 4.2 (Bio) + HF6 | https://www.uni-saarland.de/en/study/programmes/master/bioinformatics.html |
| 142 | Uni Bonn M.Sc. Life Science Informatics | Section 4.2 (Bio) + HF9 (1 Mar CLOSED) | https://www.uni-bonn.de/en/studying/degree-programs/degree-programs-a-z/life-science-informatics-msc |
| 154 | Uni Siegen M.Sc. CS — Medical Informatics track | Section 4.2 (Med Inf) | https://www.uni-siegen.de/en/study/master/computer-science |
| 164 | Uni Lübeck M.Sc. Medical Informatics | Section 4.2 (Med Inf) | https://www.uni-luebeck.de/en/university-education/degree-programmes/ |
| 168 | Uni Hamburg M.Sc. Bioinformatics | Section 4.2 (Bio) | https://www.inf.uni-hamburg.de/en/studies/master/bioinf.html |
| 183 | MLU Halle M.Sc. Bioinformatik | Section 4.2 (Bio) | https://studienangebot.uni-halle.de/bioinformatik-master-120 |
| 46 | HPI M.Sc. Digital Health | Section 4.2 (Med Inf-leaning) | https://hpi.de/en/studies/before-your-studies/degree-programs/master.html |
| 68 | OVGU M.Sc. Medical Systems Engineering | Section 4.2 (Med Inf) | https://uni-magdeburg.de/unimagdeburg/en/Study/Study+Programmes/Master/Medical+Systems+Engineering-p-17659.html |
| 93 | FAU M.Sc. Medical Engineering | Section 4.2 (Med Eng) + HF6 | https://www.fau.eu/degree-program/medical-engineering-m-sc |

#### Information Systems / Wirtschaftsinformatik (business)

| # | Program | Reason | URL |
|---|---|---|---|
| 91 | FAU M.Sc. International Information Systems | Section 4.2 (business IS) + HF6 | https://www.fau.eu/degree-program/international-information-systems-iis-m-sc |
| 95 | Uni Passau M.Sc. Information Systems | Section 4.2 (business IS) | https://www.uni-passau.de/en/msc-infosys |
| 143 | Uni Münster M.Sc. Information Systems | Section 4.2 (business IS) | https://www.wi.uni-muenster.de/prospective-students/our-courses-study/master-science-information-systems |
| 148 | Uni Köln M.Sc. Information Systems | Section 4.2 (business IS) | https://wiso.uni-koeln.de/en/studies/master/master-information-systems |

#### Computational Linguistics / NLP / Language Tech (standalone)

| # | Program | Reason | URL |
|---|---|---|---|
| 50 | Uni Potsdam M.Sc. Cognitive Systems | Section 4.2 (Cog/Comp Ling) | https://www.ling.uni-potsdam.de/cogsys/ |
| 77 | LMU M.Sc. Computational Linguistics | Section 4.2 (Comp Ling) | https://www.cis.uni-muenchen.de/ |
| 112 | Uni Tübingen M.A. Computational Linguistics | Section 4.2 (Comp Ling) | https://uni-tuebingen.de/studium/studienangebot/verzeichnis-der-studiengaenge/detail/course/computerlinguistik-computational-linguistics-master/ |
| 133 | USaar M.Sc. LCT | Section 4.2 (Comp Ling) + HF6 | https://www.uni-saarland.de/en/study/programmes/master/lct.html |
| 134 | USaar M.Sc. LST | Section 4.2 (Comp Ling) + HF6 | https://www.uni-saarland.de/en/study/programmes/master/lst.html |
| 178 | Uni Trier M.Sc. NLP | Section 4.2 (NLP standalone) | https://www.uni-trier.de/en/studium/studienangebot/studiengaenge-von-a-z/english-taught-masters-courses-1/natural-language-processing-master-of-science-1-subject-study-information-en |

#### Geoinformatics

| # | Program | Reason | URL |
|---|---|---|---|
| 103 | Uni Augsburg M.Sc. Geoinformatics | Section 4.2 (Geoinformatics) | https://www.uni-augsburg.de/en/studium/studienangebot/uebersicht/geoinformatics-msc/ |
| 144 | Uni Münster M.Sc. Geoinformatics and Spatial Data Science | Section 4.2 (Geoinf) | https://www.uni-muenster.de/Geoinformatics/en/studying/msc/index.html |

#### Cognitive Science (non-CS faculty)

| # | Program | Reason | URL |
|---|---|---|---|
| 113 | Uni Tübingen M.Sc. Cognitive Science | Section 4.2 (Cog Sci) | https://uni-tuebingen.de/en/study/finding-a-course/degree-programs-available/detail/course/cognitive-science-master/ |
| 172 | Uni Osnabrück M.Sc. Cognitive Science | Section 4.2 (Cog Sci, non-CS faculty) | https://www.ikw.uni-osnabrueck.de/en/prospective_students/master_cognitive_science.html |
| 173 | Uni Osnabrück M.Sc. Cognitive Computing | Section 4.2 (Cog Sci) + HF5 fail (€5,000/sem) | https://www.uni-osnabrueck.de/en/studying/our-study-programs/study-programs-from-a-z/cognitive-computing-master-of-science-part-time |

#### Discontinued

| # | Program | Reason | URL |
|---|---|---|---|
| 19 | TU Dresden M.Sc. Distributed Systems Engineering | Standalone discontinuing → track in MSc CS | https://tu-dresden.de/ing/informatik/studium/studienangebot/master-studiengaenge/distributed-systems-engineering |
| 21 | TU Dresden M.Sc. Computational Logic | Closing to new applicants — verify | https://tu-dresden.de/ing/informatik/studium/studienangebot/master-studiengaenge/master-computational-logic |
| 79 | LMU M.Sc. Data Science (Elite) | Discontinued (last intake WS 24/25) | https://www.m-datascience.mathematik-informatik-statistik.uni-muenchen.de/ |

---

## NEAR-MISSES — Section 9.10 (separate file)

These programs almost qualify but have one issue worth applicant review. Will be detailed in `10_near_misses.md`.

| # | Program | Issue | URL |
|---|---|---|---|
| 1 | RWTH M.Sc. Computer Science | WS 26/27 closed (1 Mar) + GRE; Summer 27 application opens 1 Jun 2026 | https://www.informatik.rwth-aachen.de/cms/informatik/studium/vor-dem-studium/~nhhb/masterstudiengaenge/?lidx=1 |
| 136 | RPTU M.Sc. Computer Science | WS 26/27 closed (30 Apr); SS27 deadline 31 Oct 2026 → backup tier | https://applymsc.informatik.uni-kl.de/ |
| 30 | Uni Stuttgart M.Sc. CS | WS 26/27 closed (15 Jan); SS27 deadline 15 Jul 2026 → backup tier | https://www.uni-stuttgart.de/en/study/study-programs/Computer-Science-M.Sc.-00001/ |
| 10 | TU Berlin M.Sc. ICT Innovation | EIT Digital double-degree, separate process; flag for applicant interest | https://www.tu.berlin/studieren/studienangebot/gesamtes-studienangebot/studiengang/ict-innovation-m-sc |
| 156 | UDE M.Sc. Computer Engineering | German B2 needed at enrollment — applicant could realistically reach if 14 mo lead | https://www.uni-due.de/iw/en/study/m-ce.php |
| 108 | Uni Tübingen M.Sc. CS | German B2-C1 required — too high for applicant currently | https://uni-tuebingen.de/en/study/finding-a-course/degree-programs-available/detail/course/computer-science-master/ |
| 106 | Uni Heidelberg M.Sc. Scientific Computing | Deadline ambiguous (15 Mar vs 30 Sep) — verify in Phase 3; could be open | https://www.uni-heidelberg.de/en/study/all-subjects/scientific-computing/scientific-computing-master |
| 107 | Uni Heidelberg M.Sc. Computer Engineering | Deadline 30 Sep WS — verify CS-content vs HW-content for scope | https://www.uni-heidelberg.de/en/study/all-subjects/computer-engineering/computer-engineering-master |

---

## KEEP — Programs surviving Phase 2 (move to Phase 3 deep verification)

| # | University | Program | Deadline (provisional) | Tuition | Initial tier guess | URL |
|---|---|---|---|---|---|---|
| 8 | TU Berlin | M.Sc. Computer Science | 31 Aug 2026 | free | Reach (brand) | https://www.tu.berlin/en/eecs/academics-teaching/study-offer/masters-programs/msc-computer-science-informatik |
| 12 | TU Darmstadt | M.Sc. Computer Science | 15 Jul 2026 | free | Reach/Target | https://www.informatik.tu-darmstadt.de/studium_fb20/im_studium/studiengaenge_liste/computer_science_msc.en.jsp |
| 14 | TU Darmstadt | M.Sc. IT Security | 15 Jul 2026 | free | Target | https://www.informatik.tu-darmstadt.de/studium_fb20/im_studium/studiengaenge_liste/itsecurity_msc.en.jsp |
| 15 | TU Darmstadt | M.Sc. AI and Machine Learning | 15 Jul 2026 | free | Reach (AI prestige) | https://www.informatik.tu-darmstadt.de/studium_fb20/im_studium/studiengaenge_liste/aim_msc.en.jsp |
| 16 | TU Darmstadt | M.Sc. Distributed Software Systems | 15 Jul (verify) | free | Target | https://www.informatik.tu-darmstadt.de/studium_fb20/vor_dem_studium/uebersicht_studiengaenge/index.en.jsp |
| 17 | TU Darmstadt | M.Sc. Visual Computing | unverified (verify standalone vs track) | free | Target (VC fit) | https://www.informatik.tu-darmstadt.de/studium_fb20/vor_dem_studium/uebersicht_studiengaenge/index.en.jsp |
| 18 | TU Dresden | M.Sc. Computer Science | 15 Jul 2026 | free | Target | https://tu-dresden.de/ing/informatik/studium/studienangebot/master-studiengaenge/m-sc-computer-science |
| 20 | TU Dresden | M.Sc. Computational Modeling and Simulation | 15 Jul (verify) | free | Target (Visual Computing track) | https://tu-dresden.de/ing/informatik/studium/studienangebot/master-studiengaenge/computational-modeling-and-simulation |
| 23 | TU Hamburg | M.Sc. Computer Science | 15 Jul 2026 | free | Target | https://www.tuhh.de/tuhh/en/studying/before-studying/degree-courses/masters-programs/computer-science |
| 24 | TU Hamburg | M.Sc. Computer Science in Engineering | 15 Jul 2026 | free | Target | https://www.tuhh.de/tuhh/en/studying/before-studying/degree-courses/masters-programs/computer-science-in-engineering |
| 25 | TU Hamburg | M.Sc. Information and Communication Systems | 15 Jul (verify) | free | Target/Safety | https://www.tuhh.de/tuhh/en/studying/before-studying/degree-courses/international-study-programs/information-and-communication-systems |
| 33 | Leibniz Hannover | M.Sc. Computer Science | 31 May 2026 | free | Target | https://www.uni-hannover.de/en/studium/studienangebot/info/studiengang/detail/computer-science-1 |
| 34 | Leibniz Hannover | M.Sc. AI-driven Mechatronics & Robotics | 31 May 2026 | free | Target (AI fit) | https://www.uni-hannover.de/en/studium/studienangebot/info/studiengang/detail/ai-driven-mechatronics-and-robotics |
| 43 | HPI Potsdam | M.Sc. Computer Science | 1 Jun 2026 | free | Target/Reach | https://hpi.de/en/studies/computer-science-msc/ |
| 44 | HPI Potsdam | M.Sc. Cybersecurity | 1 Jun 2026 (verify standalone) | free | Target | https://hpi.de/en/studies/before-your-studies/degree-programs/master.html |
| 47 | HPI Potsdam | M.Sc. IT-Systems Engineering | 1 Jun 2026 (verify standalone) | free | Target | https://hpi.de/en/studies/before-your-studies/degree-programs/master.html |
| 48 | HPI Potsdam | M.Sc. Software Systems Engineering | 1 Jun 2026 (verify) | free | Target | https://hpi.de/en/studies/before-your-studies/degree-programs/master.html |
| 49 | Uni Potsdam | M.Sc. Computer Science | 15 Jul (verify) | free | Target/Safety | https://www.uni-potsdam.de/en/studium/what-to-study/master/computer-science |
| 51 | BTU | M.Sc. Computer Science | 15 Jul 2026 | free | Safety | https://www.b-tu.de/en/informatik-ms |
| 52 | BTU | M.Sc. Artificial Intelligence | 15 Jul 2026 | free | Safety (AI fit) | https://www.b-tu.de/en/artificial-intelligence-ms |
| 53 | BTU | M.Sc. Cyber Security | 15 Jul 2026 | free | Safety | https://www.b-tu.de/en/cybersecurity-ms |
| 54 | BTU | M.Sc. Information and Media Technology | unverified | free | Safety | https://www.b-tu.de/en/imt-ms |
| 55 | TU Chemnitz | M.Sc. Computer Science | 15 Jul 2026 | free | NEAR-MISS / Safety | https://www.tu-chemnitz.de/informatik/studium/studiengaenge/ma_informatik.php.en — verify A1 German timing in Phase 3 (Section 12) |
| 56 | TU Chemnitz | M.Sc. Web Engineering | 15 Jul 2026 | free | Safety | https://www.tu-chemnitz.de/informatik/studium/studiengaenge/ma_web_engineering.php.en |
| 57 | TU Chemnitz | M.Sc. Automotive Software Engineering | 15 Jul 2026 | free | Safety | https://www.tu-chemnitz.de/informatik/studium/studiengaenge/ma_automotive_software_engineering.php.en |
| 58 | TU Chemnitz | M.Sc. Embedded Systems | 15 Jul 2026 | free | Safety | https://www.tu-chemnitz.de/etit/studium/stugang/index.php.en?page=m_es |
| 59 | TU Chemnitz | M.Sc. Information and Communication Systems | 15 Jul (verify) | free | Safety | https://www.tu-chemnitz.de/etit/studium/stugang/?page=m_is |
| 60 | TU Ilmenau | M.Sc. Research in Computer & Systems Engineering | 15 May 2026 (non-EU) | free + €75 fee | Safety | https://www.tu-ilmenau.de/en/study/before-the-study/range-of-courses/master/research-in-computer-systems-engineering-msc |
| 62 | TU Ilmenau | M.Sc. Communications and Signal Processing | 15 May (likely, non-EU) | free | Safety | https://www.tu-ilmenau.de/en/study/before-the-study/range-of-courses/master/communications-and-signal-processing-msc |
| 65 | OVGU Magdeburg | M.Sc. Digital Engineering | 15 May 2026 | free | Safety | https://www.ovgu.de/unimagdeburg/en/Study/Study+Programmes/Study+Programmes+in+English/Digital+Engineering-p-17626.html |
| 67 | OVGU Magdeburg | M.Sc. Visual Computing | 15 May 2026 | free | Safety (VC fit!) | https://www.ovgu.de/unimagdeburg/en/Study/Study+Programmes/Master/Visual+Computing-p-17624.html |
| 70 | Uni Bremen | M.Sc. AI and Intelligent Systems | unverified | free | Target (AI fit) | https://www.uni-bremen.de/en/studies/orientation-application/offered-study-program/dbs/study/324 |
| 72 | Uni Bremen | M.Sc. Digital Media | 31 May 2026 | free | Target (VC fit) | https://digitalmedia-bremen.de/profile/master/ |
| 71 | Uni Bremen | M.Sc. CIT | likely 15 Jul (verify) | free | Safety — flag German class sem 1 | https://www.uni-bremen.de/en/faculty-1-physics-electrical-engineering/studies/degree-programs/communication-and-information-technology-cit-msc |
| 94 | Uni Passau | M.Sc. Computer Science | 31 May 2026 | free | Target | https://www.uni-passau.de/en/msc-computer-science |
| 96 | Uni Bayreuth | M.Sc. Computer Science | 17 Jul 2026 | free | Target — GPA 2.5 cutoff (applicant 2.4 just clears) | https://www.uni-bayreuth.de/en/master/computer-science |
| 99 | Uni Würzburg | M.Sc. Computer Science | 17 Jul 2026 | free | Target | https://www.informatik.uni-wuerzburg.de/en/studies/degree-programmes/master-computer-science/ |
| 100 | Uni Augsburg | M.Sc. Computer Science | 10 Aug 2026 | free | Target — verify HF4 (German A2) | https://www.uni-augsburg.de/en/studium/studienangebot/uebersicht/computer-science-msc/ |
| 101 | Uni Augsburg | M.Sc. Software Engineering Elite | unverified | free | Reach (Elite Network) | https://www.uni-augsburg.de/en/studium/studienangebot/uebersicht/software-engineering-elite-graduate-programme-msc/ |
| 102 | Uni Augsburg | M.Sc. Computer Science in Engineering | unverified | free | Target | https://www.uni-augsburg.de/en/fakultaet/fai/informatik/studienangebot/msc-inginf/ |
| 104 | Uni Regensburg | M.Sc. Computer Science | 1 Jun 2026 | free | Target | https://www.uni-regensburg.de/en/informatics-data-science/study/prospective-students/msc-computer-science |
| 114 | Uni Freiburg | M.Sc. Computer Science | 1 Jun 2026 (non-EU) | €1,500/sem | Reach (brand + AI track) | https://www.tf.uni-freiburg.de/en/study-programs/computer-science/m-sc-computer-science |
| 116 | Uni Ulm | M.Sc. Computer Science | 18 Jul 2026 | €1,500/sem | Target | https://www.uni-ulm.de/en/in/faculty/studies/courses/study-course/course/computer-science-master/ |
| 117 | Uni Ulm | M.Sc. Computational Science and Engineering | unverified | €1,500/sem | Target | https://www.uni-ulm.de/en/study/study-at-ulm-university/study-programmes/course-information/course/computational-science-and-engineering-master/ |
| 121 | Uni Mainz | M.Sc. Computational Sciences | unverified | free | NEAR-MISS — verify language | https://www.studium.uni-mainz.de/en/choosing-your-degree-program/courses-offered/computational-sciences-msc/ |
| 123 | Uni Marburg | M.Sc. Computer Science | 15 Jul 2026 | free | Safety/Target | https://www.uni-marburg.de/en/studying/after-your-first-degree/masters-programs/degree-programs/computer-science-msc |
| 140 | Uni Bonn | M.Sc. Computer Science | **15 May–1 Jun 2026 (non-EEA)** | free | Reach (brand) — extreme deadline | https://www.informatik.uni-bonn.de/en/studies/master-programs/master-computer-science/msc-cs |
| 141 | Uni Bonn | M.Sc. Cyber Security | 15 May–1 Jun 2026 | free | Target — extreme deadline | https://www.informatik.uni-bonn.de/en/studies/master-programs/master-cyber-security/msc-cysec |
| 146 | Uni Köln | M.Sc. Computational Sciences | 15 Jul 2026 | free | Target | https://mathnat.uni-koeln.de/en/studies/master/computational-sciences |
| 149 | Uni Paderborn | M.Sc. Computer Science | 31 May 2026 | free | Target | https://www.uni-paderborn.de/en/studyoffer/course_of_study/computer-science-master |
| 150 | Uni Paderborn | M.Sc. Computer Engineering | 31 May 2026 | free | Target | https://www.uni-paderborn.de/en/studyoffer/course_of_study/computer-engineering-master |
| 151 | Uni Siegen | M.Sc. CS — Visual Computing track | unverified (portal opens 1 Jan 2026; lang cert 30 Apr) | free | Safety (VC fit!) | https://www.uni-siegen.de/en/eti-international-master-in-computer-science-visual-computing |
| 152 | Uni Siegen | M.Sc. CS — CISS track | unverified | free | Safety | https://www.uni-siegen.de/en/eti-international-master-in-computer-science |
| 153 | Uni Siegen | M.Sc. CS — Embedded Systems track | unverified | free | Safety | https://www.uni-siegen.de/en/eti-international-master-in-computer-science-embedded-systems |
| 157 | Uni Bielefeld | M.Sc. Intelligent Systems / IISY | 15 Jul 2026 | free | Target (AI fit) | https://www.uni-bielefeld.de/fakultaeten/technische-fakultaet/studium/master/iisy/ |
| 159 | Uni Lübeck | M.Sc. Computer Science | 15 Jul 2026 | free | Safety/Target | https://www2.uni-luebeck.de/en/study-program/computer-science-and-mathematics/information-technology/masters-program-in-computer-science/ |
| 160 | Uni Lübeck | M.Sc. IT Security | 15 Jul 2026 | free | Safety/Target | https://www.uni-luebeck.de/en/university-education/degree-programmes/it-security/masters-degree/profile.html |
| 161 | Uni Lübeck | M.Sc. Robotics and Autonomous Systems | 15 Sep 2026 EU; non-EU likely earlier | free | Target (AI fit) | https://www2.uni-luebeck.de/en/study-program/technology/robotics-and-autonomous-systems/masters-degree-program-robotics-and-autonomous-systems/ |
| 162 | Uni Lübeck | M.Sc. Media Informatics | unverified | free | Safety | https://www2.uni-luebeck.de/en/study-program/computer-science-and-mathematics/media-informatics/masters-degree-program-in-media-informatics/ |
| 165 | Uni Hamburg | M.Sc. Intelligent Adaptive Systems | unverified (typically 31 Mar) | free | NEAR-MISS — verify deadline; possibly closed | https://www.inf.uni-hamburg.de/en/studies/master/ias.html |
| 169 | TU Braunschweig | M.Sc. Computational Sciences in Engineering | 15 Jul 2026 | free | Target | https://www.tu-braunschweig.de/en/cse |
| 174 | Uni Rostock | M.Sc. Computer Science International | 1 Apr–31 May 2026 | free | Safety | https://www.informatik.uni-rostock.de/studium-lehre/master-studiengaenge/computer-science-international/ |
| 175 | Uni Rostock | M.Sc. Computational Science and Engineering | 31 May 2026 | free | Safety | https://www.ief.uni-rostock.de/en/studiengaenge/master-studiengaenge-2/computational-science-and-engineering-msc/cse-master-spso-2018/ |
| 176 | Uni Kiel (CAU) | M.Sc. Computer Science (English) | 15 Jul / 1 Aug 2026 | free | Target | https://www.inf.uni-kiel.de/en/studies/programs/computer-science-master-program-in-english |
| 184 | Uni Kassel | M.Sc. Computer Science | 15 Jul 2026 | free | Target — verify English-since-WS-26/27 | https://www.uni-kassel.de/uni/en/studium/computer-science-master.html |
| 185 | Uni Göttingen | M.Sc. Applied Computer Science | unverified (15 May likely for non-EU) | free | Target — verify HF4 mandatory German modules | https://www.uni-goettingen.de/en/applied+computer+science+%28m.sc.%29/673944.html |

**KEEP count: 64 programs across ~30 universities** (some universities contribute 3-5 programs).

This will reduce further in Phase 3 once each program's exact deadline, language requirements, and GRE/GATE rule are verified from the Tier A page.

---

## Phase 2 summary

- **Inventory:** 185 program rows
- **EXCLUDED:** ~110 programs across HF5/HF6/HF9/HF2 + Section 4.2
- **NEAR-MISS:** ~8 programs (mostly closed for WS 26/27, with SS27 backup or German requirement just out of reach)
- **KEPT:** 64 programs → Phase 3 deep verification

**Universities with no surviving program:**
- TU München (HF5)
- KIT (HF6 + HF2)
- RWTH Aachen (HF9 + HF6 — backup tier only)
- Uni Stuttgart (HF9 — backup tier only)
- LMU München (HF2)
- FAU (HF6)
- Universität des Saarlandes (HF6)
- Universität Konstanz (HF6 + HF9)
- HU Berlin (HF2)
- FU Berlin (HF2)
- Uni Heidelberg (HF9 + Section 4.2; Computer Engineering near-miss)
- Uni Tübingen (HF4 + HF9)
- Uni Trier (Section 4.2 — only English programs out-of-scope)
- Uni Münster (HF2 / Section 4.2)
- Uni Mainz (HF2)
- Uni Jena (HF2)
- MLU Halle (HF2)
- TU Braunschweig MSc Inf (HF2 — but CSE kept)
- Uni Duisburg-Essen (HF4)
- Uni Osnabrück (Section 4.2)
- Goethe Frankfurt (HF9)
- Universität Hamburg main MSc Informatik (HF2 — but IAS kept as near-miss)
- RPTU Kaiserslautern (HF9 — backup tier)

**Universities with 1+ surviving programs:** TU Berlin, TU Darmstadt, TU Dresden, TUHH, Leibniz Hannover, HPI, Uni Potsdam, BTU Cottbus, TU Chemnitz, TU Ilmenau, OVGU, Uni Bremen, Uni Passau, Uni Bayreuth, Uni Würzburg, Uni Augsburg, Uni Regensburg, Uni Freiburg, Uni Ulm, Uni Mainz (Computational only), Uni Marburg, Uni Bonn, Uni Köln, Uni Paderborn, Uni Siegen, Uni Bielefeld, Uni Lübeck, TU Braunschweig (CSE), Uni Rostock, Uni Kiel, Uni Kassel, Uni Göttingen, Uni Hamburg (IAS near-miss).

→ Phase 3 begins next: deep verification of the 64 KEEP programs from Tier A pages.
