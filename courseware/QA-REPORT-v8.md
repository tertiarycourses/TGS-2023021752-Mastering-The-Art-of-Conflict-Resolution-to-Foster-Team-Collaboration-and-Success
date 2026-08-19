# Courseware QA Report — v8.0

**Course:** Mastering The Art of Conflict Resolution to Foster Team Collaboration and Success  
**Course code:** TGS-2023021752  
**QA date:** 20 August 2026  
**Release result:** PASS

## Release inventory

| Component | Result |
|---|---:|
| Master trainer slide deck | 129 slides; PPTX and PDF |
| Learner Guide | 30 pages; DOCX and PDF |
| Lesson Plan | 10 pages; DOCX and PDF |
| Activities | 8 individual folders; 25 Markdown files, 25 matching PDFs and 8 editable sample PPTX artefacts |
| Written Assessment (SAQ) | Candidate paper and answer key; 6 open-ended questions; K1–K6 covered |
| Case Study Assessment | Candidate paper and answer key; 4 open-ended questions; A1–A9 covered |

## Content and alignment checks

- Useful coverage from the reference deck was retained and expanded through the approved source set.
- Concepts, cases and tools cover conflict signals, root causes, communication, style choice, mediation, negotiation, leadership intervention, policy and ethics, escalation, implementation and review.
- Each activity uses a realistic Singapore workplace case with named roles, scenario data, questions, observer criteria, evidence requirements and an artefact to submit.
- Detailed procedures appear in the Learner Guide and activity packs, not in the presentation.
- No practice exam content is present.
- Learner-facing terminology uses **activities**; there is no learner-facing `labs` folder.
- Source traceability is documented in `SOURCE-COVERAGE-v8.md`.

## Presentation QA

- Confirmed 129 slides, within the 100–150 slide requirement.
- Confirmed topic-specific generated cover art, all-white house style, readable visual hierarchy and two trainer profile cards.
- Confirmed front and end TRAQOM digital attendance, front assessment briefing, end assessment flow, activity access and required final slide order.
- Confirmed the deck contains no detailed step-by-step activity instructions.
- Full contact-sheet review completed after repair of the common footer, source-line placement, colour contrast, crowded cards, recap balance and trainer-profile placeholder.
- Final slide order: Assessment → Assessment Flow → Digital Attendance → Thank You.

## Learner Guide and Lesson Plan QA

- Static, page-numbered contents pages are populated in both documents.
- Long tables repeat their headers and do not leave clipped or unlabeled continuation rows.
- Activity headings, role sections, debrief sections and artefact requirements are kept with their following content.
- Version-control tables were widened and page use rebalanced.
- Rendered PDFs were inspected after the DOCX repairs: Learner Guide 30 pages; Lesson Plan 10 pages.

## Activity-pack QA

- Eight activity directories are present and independently usable.
- Every activity contains `INSTRUCTIONS`, `WORKSHEET` and `CHECKLIST` in both Markdown and PDF.
- Markdown/PDF filename parity passed: 25 Markdown files and 25 matching PDFs.
- Every activity includes an editable sample artefact in PPTX format.

## Assessment QA

- Written Assessment: 1 hour; 6 open-ended questions; K1–K6 coverage complete.
- Case Study Assessment: 1 hour; 4 open-ended questions; A1–A9 coverage complete.
- Candidate-paper and answer-key page structure, cover pages, instructions, marking guidance and answer spaces passed rendered inspection.
- Rendered page counts: WA candidate 4, WA answer key 7, CS candidate 6, CS answer key 5.
- Candidate papers are learner-accessible; answer keys are excluded from learner links and stored in a Drive limited-access trainer-only subfolder.

## Publication QA

- Google Drive destination identity was verified before upload.
- A dry run was reviewed before the first write; superseded files were archived rather than deleted.
- A final idempotent Drive push reported all published artefacts unchanged and no activity files copied or archived.
- Direct permission checks passed for both candidate papers as public learner files.
- Direct permission and anonymous-download checks confirmed both answer keys are not publicly downloadable.
- TMS dry-run and secure before/after verification passed for seven intended links; unrelated course fields were unchanged.
- `.env` records the verified courseware folder link.

## Tooling note

The optional standalone OOXML validator could not start because its installed `validators` Python package import was unavailable. This was not treated as a pass. The actual PPTX and DOCX packages opened successfully, converted successfully through LibreOffice and passed rendered visual inspection and targeted content checks.
