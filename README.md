# GermanGrammarly

> A complete, structured self-study repository for German grammar — from absolute beginner (A1) through intermediate (B1) — built on the spine of *Grammatik aktiv A1-B1* (Cornelsen).

## Overview

This repository is a **content-first German learning project**, not a software project. It contains a fully structured, bilingual (English + Vietnamese) grammar curriculum covering **all 80 chapters** of the *Grammatik aktiv A1-B1* textbook, organized into three progressive levels.

| Level | Chapters | Modules | Status |
|---|---|---|---|
| **A1** (Beginner) | Kap. 1-22 | 12 modules | ✅ 100% Complete |
| **A2** (Elementary) | Kap. 23-48 | 15 modules | ✅ 100% Complete |
| **B1** (Intermediate) | Kap. 49-80 | 19 modules | ✅ 100% Complete |

**Total: 46 modules · 270+ files · Kapitel 1-80 fully covered** 🏆

## Who This Repository Is For

This repo is useful if you are:

- a complete beginner starting German from scratch
- an A1/A2/B1 learner preparing for **Goethe / ÖSD / telc** style exams
- a self-learner who wants a study path, not isolated grammar notes
- a tutor building lessons from an existing grammar spine
- a learner who wants English explanations with Vietnamese support

## Repository Structure

```text
GermanGrammarly/
├── README.md                              ← You are here
├── german-a1-curriculum/                  ← Quick-start A1 (6 lessons)
│   ├── 01-nouns-articles/ ... 06-modal-verbs/
│   ├── a1-exam-prep/
│   ├── a1-expanded-course/
│   └── study-plan-21-days.md
├── A1-grammatik-aktiv/                    ← Book-aligned A1 (Kap. 1-22)
│   ├── M01-erste-schritte/ ... M12-uhrzeit-datum-exam/
│   ├── CURRICULUM-MAP.md
│   └── STUDY-ROADMAP.md
├── A2-grammatik-aktiv/                    ← Book-aligned A2 (Kap. 23-48)
│   ├── M01-praeteritum-sein-haben/ ... M15-verben-genus/
│   ├── CURRICULUM-MAP.md
│   └── STUDY-ROADMAP.md
├── B1-grammatik-aktiv/                    ← Book-aligned B1 (Kap. 49-65)
│   ├── M01-relativsaetze/ ... M13-n-deklination-adjektive-nomen/
│   ├── CURRICULUM-MAP.md
│   └── STUDY-ROADMAP.md
├── ROADMAP_Grammatik_Aktiv_A1_B1_EN.md    ← Full book roadmap (English)
└── ROADMAP_Grammatik_Aktiv_A1_B1.md       ← Full book roadmap (Vietnamese)
```

---

## 🟢 Track 1: Quick-Start A1 — `german-a1-curriculum/`

A compact, self-contained 6-lesson A1 curriculum. Best if you want the fastest possible start.

| Lesson | Topic |
|---|---|
| 1 | Nouns, articles, gender, and plurals |
| 2 | Personal pronouns, `sein`, `haben`, possessives |
| 3 | Present tense and separable verbs |
| 4 | Word order, questions, and negation |
| 5 | Cases and prepositions |
| 6 | Modal verbs, imperative, time expressions, and connectors |

Supporting resources: `vocabulary.md` · `memorization-tips.md` · `study-plan-21-days.md` · `practice-test.md` · `a1-exam-prep/` · `a1-expanded-course/`

---

## 🔵 Track 2: Book-Aligned Curriculum — The Main Path

This is the primary curriculum, following the exact chapter progression of *Grammatik aktiv A1-B1*. Each level has its own directory with a README, Curriculum Map, and Study Roadmap.

### A1: Foundation (Kapitel 1-22) — [Open A1](A1-grammatik-aktiv/README.md)

| Module | Focus |
|---|---|
| M01 | Personal pronouns & Erste Schritte |
| M02 | Present tense conjugation |
| M03 | sein, haben, special verbs, vowel change |
| M04 | Modal verbs |
| M05 | Separable verbs and imperative |
| M06 | Questions and word order |
| M07 | Nouns, articles, plural |
| M08 | Negation |
| M09 | Accusative and dative |
| M10 | Possessives, welcher/dieser, object pronouns |
| M11 | Verbs with accusative and dative |
| M12 | Time, dates, and exam-facing consolidation |

### A2: Expansion (Kapitel 23-48) — [Open A2](A2-grammatik-aktiv/README.md)

| Phase | Modules | Focus |
|---|---|---|
| Phase 1 | M01-M04 | Past Tense System & Reflexive Verbs |
| Phase 2 | M05-M08 | Präpositionen (temporal, Dativ/Akk, Wechsel, lokal) |
| Phase 3 | M09-M10 | Adjektivdeklination & Komparativ/Superlativ |
| Phase 4 | M11-M12 | Satzverbindungen & Nebensätze |
| Phase 5 | M13-M15 | Lokale Adverbien, Wortbildung, Genus-Regeln |

### B1: Mastery (Kapitel 49-65 + Supplementary) — [Open B1](B1-grammatik-aktiv/README.md)

| Phase | Modules | Focus |
|---|---|---|
| Supplementary | M01-M04 | Relativsätze, Infinitiv mit zu, als/wenn, Modalpartikeln |
| Phase 1 | M05-M07 | Präteritum erweitert, Plusquamperfekt, Reflexivpronomen (Dat), Trennbar/Untrennbar, Verben mit Präpositionen |
| Phase 2 & 3 | M08-M10 | Konjunktiv II, Passiv (Vorgangspassiv), Futur I & werden |
| Phase 4 | M11-M13 | Das Verb "lassen", Positionsverben & Genitiv, N-Deklination & Adjektive als Nomen |
| Phase 5 | M14-M15 | Adjektive als neutrale Nomen, Indirekte Fragen (More in progress) |

---

## Module Architecture

Every module across all levels follows a consistent 6-file structure:

| File | Purpose |
|---|---|
| `lesson.md` | Core grammar explanation with examples |
| `exercises.md` | Graded practice exercises |
| `answers.md` | Answer key with detailed explanations |
| `vocabulary.md` | Key words grouped by theme |
| `flashcards.md` | Front/back cards for memorization |
| `exam-tips.md` | Goethe exam strategies per module |

## VS Code A1 Autocomplete

This workspace now includes A1 German snippets in `.vscode/german-a1.code-snippets` for Markdown editing.

- Type a noun lemma like `apfel`, `wohnung`, `freundin`, `buch` to insert `article + singular + plural`.
- Type a verb lemma like `sein`, `haben`, `sprechen`, `lesen`, `aufstehen` to insert the full present-tense conjugation by subject.
- For umlauts, keep using the existing shortcuts: `ae:` -> `ä`, `oe:` -> `ö`, `ue:` -> `ü`, `ss:` -> `ß`.
- Snippet suggestions are pinned to the top and quick suggestions are enabled in Markdown files.

### How To Study Each Module

1. Read `lesson.md`
2. Review `vocabulary.md`
3. Study `flashcards.md`
4. Complete `exercises.md` without checking answers
5. Check `answers.md`
6. Read `exam-tips.md`
7. Revisit weak points after 1, 3, and 7 days

---

## Recommended Learning Paths

### Path 1: Zero to A1 — Fastest Start
1. `german-a1-curriculum/README.md`
2. Lessons 01-06 in order
3. `study-plan-21-days.md` as calendar
4. `a1-exam-prep/` for exam readiness

### Path 2: Full Book-Aligned Journey (A1 → A2 → B1)
1. `A1-grammatik-aktiv/STUDY-ROADMAP.md` → Study M01-M12
2. `A2-grammatik-aktiv/STUDY-ROADMAP.md` → Study M01-M15
3. `B1-grammatik-aktiv/STUDY-ROADMAP.md` → Study M01-M13
4. Use `CURRICULUM-MAP.md` in each level to track coverage

### Path 3: Exam-Oriented (Skip to your level)
1. Go directly to your target level folder
2. Read the `STUDY-ROADMAP.md` of that level
3. Focus on modules with exam-tips that match your target exam

---

## Pedagogical Design Principles

- **Book Core vs. Expert Additions:** Each lesson clearly labels what comes from the textbook (📘 Book Core) and what is supplemented by experienced German instructors (📚 Expert Addition).
- **Bilingual Format:** English is the primary instructional language; Vietnamese translations (🇻🇳) are provided for key grammar terms, example translations, and cultural context.
- **Exam Alignment:** Every module includes specific strategies for Goethe/ÖSD/telc exams at the corresponding CEFR level.

---

## Language Style

- **English** explanations for core grammar teaching
- **German** examples, forms, and target-language content
- **Vietnamese** notes for key concepts and translations

This makes the project especially suitable for Vietnamese-speaking learners who want English-medium structure with targeted native-language support.

---

## Current Status

🏆 **The entire *Grammatik aktiv A1-B1* textbook (Kapitel 1-80) has been fully converted into this digital curriculum format.**

- ✅ A1: Kapitel 1-22 (12 modules)
- ✅ A2: Kapitel 23-48 (15 modules)
- ✅ B1: Kapitel 49-80 (19 modules)

---

## Notes About The Source Book

The curriculum materials are shaped around the progression of *Grammatik aktiv A1-B1* (Cornelsen Verlag). The included roadmap documents summarize and reorganize that book into a teachable/self-study structure.

If you publish or distribute this repository publicly, make sure you have the right to include any third-party copyrighted source files.

## License

No license file is currently present at the repository root.

If you plan to make the project public on GitHub, it is a good idea to add a license so other people know whether they can reuse, adapt, or share the materials.
