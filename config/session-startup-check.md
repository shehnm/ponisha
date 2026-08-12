# Startup Check — Session پونیشا

**هدف:** جلوگیری از فراموشی قوانین وقتی Session جدید، محیط جدید، یا فاصله زمانی بین کارها.

**محدوده:** فقط Workflow شروع و Load قوانین — **نه** تغییر Proposal Engine، **نه** Negotiation Engine.

**Single Source of Truth:** فایل‌های ریپو — **نه** حافظه گفتگو.

---

## تریگرها (قبل از هر کار مرتبط)

هر وقت کاربر گفت یا موضوع شامل بود:

- **پونیشا** / **بعدی**
- **Proposal** / پیشنهاد
- **مذاکره**
- **پروژه جدید**
- تحلیل / انتخاب / ارزیابی پروژه پونیشا

→ **Startup Check** اجرا شود (اگر در این Session هنوز انجام نشده).

---

## فایل‌های اجباری Load

قبل از ادامه، این فایل‌ها را **بخوان** (اگر در Context نیستند):

| # | فایل | نقش |
|---|------|-----|
| 1 | `AGENTS.md` | دستورالعمل agent |
| 2 | `MEMORY.md` | حافظه تأییدشده کاربر |
| 3 | `.cursor/rules/ponisha-proposals.mdc` | قانون alwaysApply |
| 4 | `config/output-format.md` | **Copy-Friendly** — فرم و متن پیشنهاد |
| 5 | `config/feasibility-check.md` | Project Selection + Feasibility + Freshness |
| 6 | `config/proposal-engine.md` | Proposal Intelligence *(اگر در ریپو موجود)* |
| 7 | `config/human-review-loop.md` | Human Review *(اگر موجود)* |
| 8 | `config/pending-bid-check.md` | ثبت «پیشنهاد دادم» *(اگر موجود)* |
| 9 | `config/architecture-freeze.md` | Freeze و Override *(اگر موجود)* |

**قانون Load:** اگر فایلی در ریپو **نیست** → در پیام startup یک خط «فایل X موجود نیست»؛ با فایل‌های موجود ادامه بده. **فرض نکن** قوانین از Session قبل در حافظه‌اند.

---

## پیام Session (فقط بار اول)

بعد از Load، در **اولین پاسخ** Session (قبل از کار اصلی) **یک خط**:

> قوانین پروژه پونیشا بررسی شد. نسخه فعلی Workflow فعال است.

- کوتاه — بدون تکرار در هر پیام بعدی
- اگر فایل مهمی نبود → همان خط + «(برخی فایل‌ها در این branch موجود نیست)»

---

## قوانین دائمی (خلاصه — جزئیات در فایل منبع)

### Copy-Friendly (Output)

هر خروجی برای Paste در پونیشا → `config/output-format.md`

- یک کلیک Copy، بدون اصلاح دستی
- فرم خط‌به‌خط؛ عنوان مراحل فقط فارسی کوتاه
- بدون جدول markdown، code fence، FA+EN نامرتب در یک خط

### Project Selection

`config/feasibility-check.md` — Fit اول، بعد Freshness، فعالیت کارفرما، رقابت.

### Human Review / Pending Bid

اگر `human-review-loop.md` / `pending-bid-check.md` موجود → قبل از Submit و بعد از «پیشنهاد دادم» رعایت شود.

---

## تضاد دستور کاربر با قوانین

1. **`config/architecture-freeze.md`** را بخوان *(اگر موجود)*
2. **تغییر معماری** (Engine، pipeline، ساختار Review) → فقط طبق قانون **Override** در Freeze — با تأیید صریح کاربر
3. **تولید Proposal / تحلیل پروژه / bid** → طبق قوانین فعلی (`output-format`، `feasibility-check`، `MEMORY`) — بدون تغییر Engine

---

## هرگز

- فرض نکن قوانین از قبل در Context فعال‌اند
- به حافظه چت به‌جای فایل ریپو تکیه کن
- Proposal Engine / Negotiation Engine را بدون درخواست صریح و رعایت Freeze تغییر بده

---

## ارجاع

- Workflow کامل agent: `AGENTS.md`
- فهرست فایل‌ها: `README.md`
