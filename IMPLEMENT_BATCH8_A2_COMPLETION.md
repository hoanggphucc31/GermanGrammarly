# Implementation Report — Batch 8: A2 Completion (Kapitel 40-48)

> **Ngày triển khai:** 2026-04-26
> **Scope:** Kapitel 40-48 (Grammatik Aktiv A1-B1)
> **Trạng thái:** ✅ Hoàn thành

---

## 1. Tổng quan

Batch 8 được làm lại để **lấp khoảng trống (gap) Kap. 40-48** bị bỏ sót trước đó, đảm bảo spine sách *Grammatik Aktiv* được triển khai liền mạch không nhảy cóc. Batch này hoàn thành toàn bộ chương trình A2 (Phase 4 & 5) với 5 modules (M11-M15), tổng cộng **30 files** song ngữ Anh-Việt.

Với Batch 8 này, **toàn bộ chương trình A2 (Kap. 23-48) đã chính thức hoàn thiện!**

---

## 2. Module Mapping (Chuẩn xác theo sách)

| Module | Thư mục | Kapitel | Tiêu đề sách | Trọng tâm |
|---|---|---|---|---|
| **M11** | `M11-satzverbindungen/` | 40-41 | *Und, oder, aber, denn / Deshalb, trotzdem, sonst, dann* | Liên từ (Position 0) & Trạng từ nối (Position 1) |
| **M12** | `M12-nebensaetze/` | 42 | *Weil, dass, wenn, ob* | Câu phụ (Nebensätze) — Động từ ở cuối câu |
| **M13** | `M13-lokale-adverbien-partikeln/` | 43-44 | *Ich bin da... / Was heißt das denn?* | Trạng từ chỉ vị trí/hướng (da/dahin, hin/her) & Tiểu từ tình thái |
| **M14** | `M14-wortbildung/` | 45-46 | *Kinderarzt / -chen, -lein, -er, -in, -ung* | Cấu tạo từ (Từ ghép Komposita & Hậu tố) |
| **M15** | `M15-verben-genus/` | 47-48 | *Ich bin dann mal weg / Der, die oder das?* | Động từ tách/không tách (nâng cao) & Quy tắc giống danh từ |

---

## 3. Cấu trúc thư mục đã tạo

Toàn bộ được đặt trong `A2-grammatik-aktiv/`:

```
A2-grammatik-aktiv/
├── M11-satzverbindungen/
│   ├── lesson.md                       ← Pos 0 (und/aber/oder/denn/sondern) vs Pos 1 (deshalb/trotzdem/sonst/dann)
│   ├── exercises.md                    ← 28 bài tập (điền từ, đảo ngữ)
│   ├── answers.md                      ← Đáp án kèm giải thích Inversion
│   ├── vocabulary.md                   ← Bảng từ vựng liên từ
│   ├── flashcards.md                   | Word order cards
│   └── exam-tips.md                    ← Sequence template cho Schreiben A2
│
├── M12-nebensaetze/
│   ├── lesson.md                       ← Quy tắc Verb-at-End với weil, dass, wenn, ob
│   ├── exercises.md                    ← 27 bài tập
│   ├── answers.md                      ← Đáp án
│   ├── vocabulary.md                   ← Signal words & verbs for dass
│   ├── flashcards.md                   | Conjunction cards & Traps (wenn vs ob)
│   └── exam-tips.md                    ← Mẹo phân biệt wenn/ob cho Goethe A2
│
├── M13-lokale-adverbien-partikeln/
│   ├── lesson.md                       ← Wo (da/dort) vs Wohin (dahin/dorthin), hin vs her, Partikeln
│   ├── exercises.md                    ← 11 bài tập trọng tâm
│   ├── answers.md                      ← Đáp án
│   ├── vocabulary.md                   ← Bảng Adverbien & Partikeln
│   ├── flashcards.md                   | Position vs Direction cards
│   └── exam-tips.md                    ← Dùng denn/mal trong Sprechen
│
├── M14-wortbildung/
│   ├── lesson.md                       ← Quy tắc Komposita (Last word rule), Suffixe (-chen, -ung, -er)
│   ├── exercises.md                    ← 19 bài tập cấu tạo từ & xác định giống
│   ├── answers.md                      ← Đáp án
│   ├── vocabulary.md                   ← Bảng Suffixe 100% đúng
│   ├── flashcards.md                   | Gender shortcut cards
│   └── exam-tips.md                    ← Mẹo đoán từ vựng trong Lesen
│
└── M15-verben-genus/
    ├── lesson.md                       ← Prefixes tách/không tách nâng cao, Mnemonic không tách (BE-ER-VER-ENT-GE-EMP)
    ├── exercises.md                    ← 20 bài tập chia Partizip II & xác định Genus
    ├── answers.md                      ← Đáp án
    ├── vocabulary.md                   ← Bảng phân loại Prefixes & Gender Suffixes
    ├── flashcards.md                   | Separable/Inseparable rule cards
    └── exam-tips.md                    ← Mẹo Partizip II không có ge-
```

---

## 4. Chi tiết Kiến thức chuyên gia (Expert Additions)

Trong quá trình implement, nội dung sách được bổ sung thêm các mẹo sư phạm để học viên dễ hiểu hơn:

| Module | Bổ sung | Lý do |
|---|---|---|
| **M11** | Phân loại rõ **Position 0 vs Position 1** | Cách dễ nhất để học viên nhớ khi nào cần đảo ngữ (Inversion), khi nào không. |
| **M12** | **The Quick Test: wenn vs ob** (when/if vs whether) | Sách thường không giải thích rõ sự khác biệt, dẫn đến lỗi dịch word-by-word. |
| **M13** | **hin vs her rule** (away vs toward speaker) | Giúp học viên định hình tư duy không gian của tiếng Đức. |
| **M14** | **The Last Word Rule** cho Komposita | Quy tắc cốt lõi nhất để xác định giống (Artikel) của từ ghép. |
| **M15** | Mnemonic **BE-ER-VER-ENT-GE-EMP-MISS-ZER** | Thần chú để nhận diện động từ không tách và không thêm `ge-` trong quá khứ. |

---

## 5. Cập nhật Navigation (Hoàn tất A2)

File `A2-grammatik-aktiv/CURRICULUM-MAP.md` đã được update:
- Cập nhật **Phase 4: Satzverbindungen & Nebensätze** (M11-M12).
- Thêm mới **Phase 5: Wortschatz & Strukturerweiterung** (M13-M15).
- Bổ sung **Communicative Functions** cho M11-M15.
- Đóng dấu hoàn tất chương trình A2.

**Trạng thái sau pass hoàn thiện (đã fix):**
- `CURRICULUM-MAP.md` ✅ đã update đúng M11-M15.
- `README.md` ✅ đã thêm Phase 4-5 với M11-M15.
- `STUDY-ROADMAP.md` ✅ đã cập nhật M11-M15 = Complete + Quick Start Links.

---

## 5.1 Những điểm đã cải thiện

### A. ✅ `README.md` và `STUDY-ROADMAP.md` đã đồng bộ

- `README.md` hiển thị đầy đủ 5 phases (M01-M15).
- `STUDY-ROADMAP.md` hiển thị 15 weeks + quick start links cho tất cả phases.

### B. ✅ Expert additions đã được ghi nhãn rõ

Các module có mở rộng đã thêm dòng **Scope** phân biệt:
- `M11/lesson.md` → 📘 Book Core: und/oder/aber/denn + deshalb/sonst/dann/danach. 📚 Expert: sondern, deswegen, trotzdem.
- `M13/lesson.md` → 📘 Book Core: Positionsadverbien + Partikeln denn/doch/mal. 📚 Expert: ja particle, hin/her.
- `M15/lesson.md` → 📘 Book Core: Zusammengesetzte Verben + Genusregeln. 📚 Expert: mnemonic, expanded suffix cheat sheet.

### C. ✅ Verdict đã chỉnh cách diễn đạt

Thay "hoàn toàn khớp với sách" bằng "bám đúng chapter spine sách" + ghi nhãn minh bạch.

---

## 6. Tổng quan Spine sách hiện tại (Đã fix lỗi)

| Level | Batch | Modules | Kap. | Trạng thái |
|---|---|---|---|---|
| **A1** | 1-4 | M01-M12 | 1-22 | ✅ Đã hoàn thành |
| **A2** | 5-7 | M01-M10 | 23-39 | ✅ Đã hoàn thành |
| **A2** | 8 | M11-M15 | 40-48 | ✅ Vừa hoàn thành (Lấp gap) |
| **B1** | Supplementary | M01-M04 | — | ✅ B1 Core Grammar (Relativsätze, Infinitiv, als/wenn) |
| **B1** | 9 (Tương lai) | M01+ | 49+ | 📋 Chờ triển khai (Präteritum erweitert, Plusquamperfekt...) |

---

## Verdict

**Batch 8 đã sửa đúng lỗi nhảy cóc spine trước đó và hiện đã bám đúng module mapping chính của sách ở `Kap. 40-48`.**

Trạng thái sau pass hoàn thiện:

- `core chapter alignment`: ✅ Đúng
- `navigation sync`: ✅ Đã đồng bộ (README, STUDY-ROADMAP, CURRICULUM-MAP đều hiển thị M11-M15)
- `strict book-only scope`: ✅ Đã ghi nhãn rõ (📘 Book Core / 📚 Expert Addition trong M11, M13, M15)

=> **Batch 8 hoàn thành. Chương trình A2 (Kap. 23-48) đã bám đúng chapter spine sách, navigation đã đồng bộ, và các phần mở rộng đã được ghi nhãn minh bạch.**
