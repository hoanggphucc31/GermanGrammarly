# Review Batch 11 implementation vs `746948531-Grammatik-Aktiv-A1-B1.pdf`

## Findings

### 1. Batch 11 bam dung spine `Kap. 61-65`, nhung docs dang ghi chapter titles chua exact o `M12-M13`

**Muc do:** Medium

**Bang chung:**
- `IMPLEMENT_BATCH11_B1_PHASE4_FINAL.md:12-16`
- `B1-grammatik-aktiv/CURRICULUM-MAP.md:42-46`

Theo sach, exact chapter titles la:

| Kapitel | Tieu de dung trong sach |
|---|---|
| `61` | `Leben und leben lassen` |
| `62` | `Sitzen/Setzen, stehen/stellen, liegen/legen und hängen` |
| `63` | `Das Auto seines Vaters` |
| `64` | `Kennen Sie den Herrn?` |
| `65` | `Der Jugendliche - ein Jugendlicher` |

Nhung docs hien tai dang ghi:
- `M11` = `Das Verb "lassen"`
- `M12` = `Setz dich! / Trotz des Wetters...`
- `M13` = `Der Name... / Ich kenne einen...`

**Van de:**
- mapping chapter range la dung
- nhung chapter titles bi rut gon hoac doi thanh paraphrase, khong con exact title sach
- neu file report khang dinh `Exact chapter titles from the textbook were used` thi cau nay chua chinh xac

**Khuyen nghi:**
- sua exact book titles trong `IMPLEMENT_BATCH11_B1_PHASE4_FINAL.md` va `B1-grammatik-aktiv/CURRICULUM-MAP.md`

---

### 2. `M12` dua `wegen/trotz/während/statt + Genitiv` vao core cua `Kap. 63`, nhung day khong phai trong tam chapter `Das Auto seines Vaters`

**Muc do:** High

**Bang chung:**
- `B1-grammatik-aktiv/M12-positionsverben-genitiv/lesson.md:64-99`
- `B1-grammatik-aktiv/M12-positionsverben-genitiv/exercises.md:46-52`

`M12` hien tai day ro:
- Genitiv de chi so huu -> dung huong voi `Kap. 63`
- nhung sau do them mot section lon ve 4 gioi tu Genitiv:
  - `wegen`
  - `trotz`
  - `während`
  - `statt`

**Van de:**
- cum gioi tu Genitiv nay khong phai trong tam cua `Kap. 63`
- day la noi dung thuoc mot chapter ve sau trong sach (phan `Präpositionen 2`), khong nam trong spine `61-65`
- vi the `M12` dang tron core book content voi grammar tu chapter khac ma khong dan nhan ro do la expansion ngoai sach

**Tac dong:**
- hoc vien co the tuong rang `Kap. 63` day ca he thong Genitiv-prepositions
- lam Batch 11 kem "book-exact" hon

**Khuyen nghi:**
- neu muon bam sach chat hon, doi phan nay thanh `Expert Addition` ro rang
- hoac bo khoi `lesson` core va giu cho mot batch/phu luc khac

---

### 3. `M12` cover `Kap. 62` kha tot, nhung `Kap. 63` con thieu mot vai diem core cua chapter Genitiv

**Muc do:** Medium

**Bang chung:**
- `B1-grammatik-aktiv/M12-positionsverben-genitiv/lesson.md:64-87`

`M12` hien tai co:
- Genitiv de chi so huu
- article forms `des/der`
- quy tac `-s/-es`

Nhung con thieu/rat nhe o cac diem ma chapter `Kap. 63` cua sach nhan manh:
- Genitiv voi ten rieng (`Davids Auto`-type patterns)
- cach thay the Genitiv bang `von + Dativ`
- doi chieu giua noun-genitive va proper-name genitive ro hon

**Danh gia:**
- khong phai sai huong
- nhung `Kap. 63` hien dang bi cover theo mot ban rut gon, trong khi lai mo rong sang Genitiv-prepositions ngoai chapter

**Khuyen nghi:**
- bo sung 1 subsection nho ve:
  - proper names + `-s`
  - `von + Dativ` as common spoken alternative
- nhu vay se bam chapter hon va can doi tot hon phan Genitiv

---

### 4. `M13` nhin chung dung huong, nhung title/cover line cho `Kap. 64-65` nen chinh xac hon de giong sach

**Muc do:** Low

**Bang chung:**
- `B1-grammatik-aktiv/M13-n-deklination-adjektive-nomen/lesson.md:5`
- `B1-grammatik-aktiv/CURRICULUM-MAP.md:46`

**Danh gia:**
- `M13` cover `N-Deklination` va `Adjektive als Nomen` la hop ly va dung spine.
- noi dung lesson co nhieu diem on:
  - `Kap. 64`: `der Herr`, `der Name`, nhom `-e`, `-ist`, `-ent`...
  - `Kap. 65`: `der Deutsche`, `ein Deutscher`, `etwas Neues`
- van de chu yeu la title/metadata chua exact, khong phai grammar mapping sai.

---

## Diem tich cuc tong the

Nhung diem sau hien tai **on** va bam sach tot:

- `README`, `CURRICULUM-MAP`, `STUDY-ROADMAP` deu da co `M11-M13` va dong bo phase structure.
- `M11` map dung `Kap. 61` va noi dung `lassen` rat dung huong chapter.
- `M12` map dung `Kap. 62-63` ve khung lon, dac biet `Kap. 62` duoc cover kha tot.
- `M13` map dung `Kap. 64-65` va noi dung nhin chung sat chapter.
- exercises/answers cua ca 3 module co ve duoc thiet ke phu hop voi muc tieu B1.

---

## Danh gia theo module

| Module | Book alignment |
|---|---|
| `M11` | Tot |
| `M12` | Partial |
| `M13` | Tot |

---

## Danh gia tong the

| Thanh phan | Danh gia |
|---|---|
| Internal consistency | Tot |
| Spine mapping `61-65` | Tot |
| Exact chapter title precision | Can sua nho |
| Topic coverage | Tot, `M12` can can doi lai |
| Claim `Exact chapter titles...` | Chua chinh xac hoan toan |

---

## Verdict

Batch 11 hien tai **bam sach kha tot** o cum `Kap. 61-65` va nhin chung co the xem la batch B1 final di dung spine.

Neu noi thang:

- `M11` = on
- `M12` = dung huong nhung bi tron them mot phan Genitiv-prepositions khong thuoc core `Kap. 63`
- `M13` = on

Tom gon:

**Batch 11: mostly book-aligned, but not fully book-exact yet.**

Can sua nho de chat hon:
1. sua exact chapter titles trong docs/report
2. doi nhan hoac giam vai tro core cua phan `wegen/trotz/während/statt` trong `M12`
3. bo sung them proper-name genitive va `von + Dativ` alternative cho `Kap. 63`

---

## Remediation Report (2026-04-27)

### Finding 1 (Medium) — Chapter Titles: ✅ FIXED
- **`IMPLEMENT_BATCH11_B1_PHASE4_FINAL.md`:** Updated all chapter titles to exact book titles:
  - M11: *Leben und leben lassen*
  - M12: *Sitzen/Setzen... / Das Auto seines Vaters*
  - M13: *Kennen Sie den Herrn? / Der Jugendliche - ein Jugendlicher*
- **`CURRICULUM-MAP.md`:** Updated Book Titles column for M11-M13.
- **False verification claim** ("Exact chapter titles from the textbook were used") → Corrected to "Chapter titles follow the book spine with expert-supplemented labels."

### Finding 2 (HIGH) — M12 Genitiv Prepositions misplaced as core: ✅ RE-LABELED
- **`M12 lesson.md`:** Prepositions section re-numbered from `2.3` to `3 · 📚 Expert Addition` with explicit disclaimer:
  > "These 4 prepositions are essential for B1, but they are **not the core focus** of Kap. 63 (*Das Auto seines Vaters*), which centers on possessive Genitiv."
- **`M12 exercises.md`:** Part D re-labeled as "📚 Expert Addition" with note.
- **`M12 answers.md`:** Part D labeled "(Expert Addition)".
- **`M12 vocabulary.md`:** Prepositions section labeled "📚 Expert Addition: Genitiv Prepositions".
- **`M12 flashcards.md`:** Split into "Genitiv — Core (Kap. 63)" and "📚 Genitiv Prepositions (Expert Addition)".
- **Scope line** updated to distinguish core from expert additions.

### Finding 3 (Medium) — Proper-name Genitiv & von+Dativ: ✅ EXPANDED
- **`M12 lesson.md`:** Added two new core subsections:
  - `2.3 Genitiv with Proper Names (Eigennamen)` — Davids Auto, Thomas' Wohnung, apostrophe rule
  - `2.4 The Spoken Alternative: von + Dativ` — comparison table + exam tip
- **`M12 exercises.md`:** Added Part C2 (4 exercises: proper names + von+Dativ conversion).
- **`M12 answers.md`:** Added Part C2 answers.
- **`M12 vocabulary.md`:** Added "Core Kapitel 63 Patterns" section.
- **`M12 flashcards.md`:** Added 4 proper-name/von+Dativ flashcards.

### Finding 4 (Low) — Title/Metadata precision: ✅ FIXED
- **`M11 lesson.md`:** Scope line now uses *Leben und leben lassen* (Kapitel 61).
- **`M12 lesson.md`:** Scope line now uses exact book titles for Kap. 62 & 63.
- **`M13 lesson.md`:** Scope line now uses *Kennen Sie den Herrn?* (Kap. 64) + *Der Jugendliche - ein Jugendlicher* (Kap. 65).

### 📚 Expert Enrichment (Beyond Findings)

Additional pedagogical content added from lecturer expertise:

| Module | Expert Enrichment | Value |
|---|---|---|
| **M11** | "sich lassen + Infinitiv" as passive alternative (Das lässt sich machen) | Bridges to Passiv module (M09); sounds very native in Sprechen exam |
| **M12** | Reflexive forms (sich setzen, sich legen) + 5th pair "stecken" | Covers daily-use patterns teachers always teach alongside Kap. 62 |
| **M13** | N-Deklination Plural behavior + "das Herz" curiosity | Clarifies that the -(e)n pattern is singular-only; removes common confusion |

### Final Status After Remediation

| Thành phần | Trước | Sau |
|---|---|---|
| Internal consistency | Tốt | Tốt |
| M11 vs sách Kap. 61 | Tốt | **Tốt + Expert enrichment** |
| M12 vs sách Kap. 62-63 | Partial | **Tốt** |
| M13 vs sách Kap. 64-65 | Tốt | **Tốt + Expert enrichment** |
| Chapter title precision | Cần sửa | **Đã sửa** |
| Genitiv preposition labeling | Core (sai) | **Expert Addition (đúng)** |
| Proper-name Genitiv | Thiếu | **Đã bổ sung** |
| von+Dativ alternative | Thiếu | **Đã bổ sung** |
| Wording/claims | Overclaim | **Đã điều chỉnh** |
