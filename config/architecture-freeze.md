# Architecture Freeze Policy

**وضعیت:** Proposal Intelligence Engine از این لحظه **Stable** است.

**تاریخ فعال‌سازی Freeze:** ۱۴۰۵/۰۵/۱۵ (۲۰۲۶-۰۸-۰۶)

---

## فایل‌های منجمد (معماری)

این فایل‌ها **نباید تغییر معماری** پیدا کنند:

| فایل |
|------|
| `config/proposal-engine.md` |
| `config/proposal-learning.md` *(ساختار و قواعد — نه داده Lesson)* |
| `config/human-review-loop.md` |
| `config/personal-voice.md` |
| `MEMORY.md` |
| `AGENTS.md` |
| `.cursor/rules/ponisha-proposals.mdc` |
| `config/output-format.md` |

### تفکیک: معماری vs داده

| مجاز (بدون解冻) | ممنوع (نیاز به شرایط زیر) |
|-----------------|---------------------------|
| ثبت Lesson در `proposal-learning` | بازنویسی pipeline یا اصول engine |
| Human Review و شمارنده تکرار | تغییر ساختار Human Review |
| ردیف `bids-log` | تغییر workflow در AGENTS/MEMORY *(مگر تأیید صریح کاربر — مثل Pending Bid Check)* |
| `last-proposal.md` / `pending-bid-check.md` | — |
| `negotiation-conversion-analysis.md` / `proposal-generation-logic-analysis.md` | — |
| sync `profile.md` | تغییر personal-voice یا output-format |
| نمونه جدید در `examples/` | تغییر Cursor Rules |

---

## شرایط رفع Freeze (هر سه باید برقرار باشد)

### ۱. حجم Proposal

حداقل **۲۰ Proposal واقعی** با این سیستم (پس از تاریخ Freeze) تولید شده باشد.

شمارنده: `proposal-learning.md` → **System Metrics**

### ۲. نتایج واقعی

حداقل **۱۰ نتیجه** ثبت شده باشد:

- برد
- باخت
- یا پاسخ کارفرما

شمارنده: `proposal-learning.md` → **System Metrics**

### ۳. مشکل تکرارشونده در داده

داده‌ها نشان دهند مشکل **تکرارشونده** وجود دارد. نمونه‌ها:

- Human Review همان ایراد را **≥ ۳ بار** ثبت کرده
- Proposal Learning الگوی شکست مشخص پیدا کرده
- نرخ پاسخ یا نرخ برد پایین‌تر از انتظار است (با داده ثبت‌شده)

---

## تا قبل از رسیدن به شرایط

agent **فقط** باید:

1. Proposal تولید کند
2. Human Review انجام دهد
3. Lesson ثبت کند
4. Learning را به‌روزرسانی کند (داده — نه معماری)

**بازطراحی معماری ممنوع.**

---

## درخواست تغییر معماری از کاربر

اگر کاربر خواست فایل منجمد را **معماری** عوض کند:

### مرحله ۱ — یادآوری

```
Architecture Freeze فعال است.

شرایط رفع Freeze:
- Proposal با این سیستم: X / ۲۰
- نتیجه ثبت‌شده: Y / ۱۰
- مشکل تکرارشونده: [بله/خیر — خلاصه]

تا رسیدن به شرایط، تغییر معماری پیشنهاد نمی‌شود.
```

### مرحله ۲ — سؤال تأیید

> «آیا با وجود فعال بودن Architecture Freeze همچنان می‌خواهید معماری تغییر کند؟»

| پاسخ | عمل |
|------|-----|
| **خیر** | معماری ثابت بماند |
| **بله** | تغییر انجام شود + یادداشت در `proposal-learning` (Override Freeze) |

**بدون تأیید صریح کاربر → تغییر معماری انجام نشود.**

---

## پیشنهاد اصلاح Engine (از Human Review ≥۳)

حتی اگر ایراد ۳ بار تکرار شد:

- **فقط پیشنهاد** به کاربر — نه تغییر خودکار
- اگر کاربر تأیید نکرد → فقط Lesson ثبت شود
- اگر هر سه شرط Freeze هم برقرار نشد → باز هم سؤال Override لازم است

---

## شمارنده‌ها

منبع رسمی: `proposal-learning.md` → بخش **System Metrics**

agent بعد از هر «پیشنهاد دادم» / «بردیم» / «باختیم» / «پاسخ داد» شمارنده را به‌روز کند.

**توجه:** bidهای قبل از تاریخ Freeze در شمارنده **نیستند** — فقط از ۱۴۰۵/۰۵/۱۵ به بعد.

---

## به‌روزرسانی این فایل

تغییر خود `architecture-freeze.md` = تغییر معماری → همان قوانین Freeze + تأیید کاربر.
