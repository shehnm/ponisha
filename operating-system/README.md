# Operating System — Shehneh Life OS

**نسخه:** 1.0 — ۱۴۰۵/۰۵/۲۱  
**زبان:** فارسی (DEC-0006)

---

## نقش

این پوشه **قوانین دائمی** Life OS را نگه می‌دارد — نه داده روزانه.

---

## فهرست سندها

| سند | موضوع |
|-----|--------|
| [agent-handoff-protocol.md](./agent-handoff-protocol.md) | استاندارد Handoff بین Cursorها |
| [data-classification.md](./data-classification.md) | FACT / GOAL / DECISION / … |
| [document-types.md](./document-types.md) | Living vs Snapshot vs Decision vs Lesson |
| [state-update-rules.md](./state-update-rules.md) | چه وقت Living Documents به‌روز شوند |
| [capacity-rules.md](./capacity-rules.md) | ظرفیت و جلوگیری از overcommitment |

---

## Life OS = Single Source of Truth

هر Agent/Cursor تخصصی:

- **می‌تواند** در repo/پوشه خودش عمیق کار کند
- **باید** Handoff به Life OS بدهد وقتی وضعیت کلان تغییر کرد
- **نباید** تصمیم مهم بدون خواندن `state/current-state.md` پیشنهاد دهد

---

## Startup Rule

→ [README-LIFE-OS.md](../README-LIFE-OS.md#startup-rule)

---

## اصل طبقه‌بندی

→ [data-classification.md](./data-classification.md)

**هیچ HYPOTHESIS به‌عنوان FACT ثبت نشود.**

---

## اصل ضد تورم

→ [document-types.md](./document-types.md)

**لینک بده، کپی نکن.**
