# پروتکل Handoff — Cursor/Agent → Life OS

**نسخه:** 1.0  
**هدف:** هر Cursor تخصصی بتواند وضعیت کلان را برای Life OS گزارش دهد.

---

## قانون

Life OS Handoff را **آرشیو خام** نمی‌کند.

Handoff باید منجر به **به‌روزرسانی Living Documents** شود (در صورت تغییر واقعی):

- `state/current-state.md`
- `priorities/current-priorities.md`
- `management-overview` مرتبط
- `finance/` در صورت اثر مالی
- `decisions/` در صورت تصمیم
- `lessons/` در صورت درس قابل تکرار

→ جزئیات: [state-update-rules.md](./state-update-rules.md)

---

## قالب Handoff

```markdown
# Handoff — [عنوان]

**حوزه:** [ponisha | odoo | book | family | finance | …]
**تاریخ:** [۱۴۰۵/…]
**منبع:** [Cursor Ponisha / ChatGPT / نویسنده / …]
**وضعیت Handoff:** [پردازش‌شده | در صف inbox | …]

---

## FACTS
- [واقعیت تأییدشده ۱]
- …

## CHANGES
- [چه چیزی تغییر کرد؟]

## DECISIONS
- [تصمیم — یا «هیچ»]

## MONEY
- [درآمد / هزینه / تعهد — یا «بدون اثر مالی»]

## COMMITMENTS
- [تعهد مشتری / خانواده — یا «بدون تعهد جدید»]

## DEADLINES
- [تاریخ مهم — یا «ندارد»]

## PENDING
- [منتظر چه چیزی؟]

## RISKS
- [ریسک — برچسب RISK]

## LESSONS
- [درس — فقط اگر قابل تکرار؛ یا «هیچ»]

## NEXT ACTION
- [اقدام بعدی دقیق]

## SOURCE OF DETAIL
- [repo / file / project ID / URL]
```

---

## جریان کار

```
Cursor تخصصی → inbox/updates.md (یا Handoff مستقیم)
            → طبقه‌بندی (FACT/DECISION/…)
            → به‌روز Living Documents
            → وضعیت inbox: «ثبت شد»
```

---

## منابع Handoff

| منبع | مسیر ورود |
|------|-----------|
| Cursor Ponisha | `inbox/updates.md` + `config/` |
| Cursor Odoo | `inbox/updates.md` |
| Cursor Book | `inbox/updates.md` |
| ChatGPT | `inbox/updates.md` |
| گزارش شخصی نویسنده | `inbox/updates.md` |

---

## مثال

→ اولین Handoff پردازش‌شده: `inbox/updates.md` — ورودی ۱۴۰۵/۰۵/۲۱ (پونیشا)
