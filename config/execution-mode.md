# Execution Mode — سیستم تحلیل کامل است

**وضعیت:** از **۱۴۰۵/۰۵/۲۹** — **Analysis System Complete**

**هدف فعلی:** **افزایش قرارداد** — نه کامل‌تر کردن سیستم.

---

## Freeze تحلیل — بدون Layer جدید

**از این مرحله به بعد:**

| ❌ ممنوع | ✅ مجاز |
|---------|---------|
| Layer / Rule / Engine / تحلیل **جدید** | **اجرای** Workflow فعلی |
| بازطراحی pipeline | ثبت **داده** (bids-log، Trace، Validation) |
| پیشنهاد «بهبود سیستم» بدون داده | تحلیل برد/باخت با **outcome واقعی** |
| تغییر معماری Engine | Lesson فقط از `[Human]` یا **مشکل تکرارشونده اثبات‌شده** |

**استثناء — Layer/Rule جدید فقط اگر:**

1. از **داده واقعی** پروژه‌ها (≥ **۳** occurrence همان مشکل — طبق `architecture-freeze.md`)
2. کاربر **صریحاً** درخواست کرد **بعد از** ارائه شواهد تکرار
3. Override Freeze طبق `architecture-freeze.md`

---

## تمرکز فعلی (۴ کار)

| # | کار | فایل‌های مرجع |
|---|-----|----------------|
| **۱** | پیدا کردن پروژه مناسب | `feasibility-check` · `project-selection-decision-analysis` · `bids-log` |
| **۲** | ارسال Proposal طبق Workflow | `ponisha-trigger` · Engine · Intent · Emotional Trust · `output-format` |
| **۳** | ثبت **همه** نتایج | `bids-log` · `project-status` · Trace · `last-proposal` |
| **۴** | تحلیل برد/باخت با داده واقعی | Conversion · Logic · **Hypothesis Validation** · `proposal-learning` |

---

## دستور «پونیشا» / «بعدی» = فقط اجرا

**کاربر گفت «پونیشا» یا «بعدی»:**

→ **`config/ponisha-trigger.md`** — **اجرا** — نه گسترش سیستم.

**Agent:**

1. Startup + Pending Bid Check
2. جستجو + Selection Analysis
3. Intent + AAL + Engine → پیش‌نویس
4. لایه‌های کیفیت (Emotional Trust + PCL + Over-Proofing)
5. **Decision Trace** (داخلی — قبل Human Review)
6. Human Review → خروجی 📋 Copy/Paste
7. **نه** پیشنهاد Layer جدید · **نه** refactor config

---

## هر Proposal — چک‌لیست اجباری

| # | الزام |
|---|--------|
| ۱ | **Copy/Paste** — `output-format.md` · 📋 code blocks |
| ۲ | **Workflow فعلی** — بدون shortcut یا حذف لایه |
| ۳ | **Decision Trace** — Trace-۱…۵ + فرضیه برد (Trace-۴) **قبل** نمایش |
| ۴ | بعد از Submit → `bids-log` + `last-proposal` |
| ۵ | بعد از outcome → **Hypothesis Validation** (HV-۱…۶) |

---

## تریگرهای outcome (ثبت + Validation)

| کاربر | عمل |
|--------|-----|
| «پیشنهاد دادم» | bids-log Submitted + Trace در Logic log |
| «پاسخ داد» | Negotiation + Conversion |
| «بردیم» / «باختیم» | Validation + learning |
| «بی‌پاسخ ماند» (نهایی) | Validation — No Response |

---

## ارجاع

- معماری Engine: `architecture-freeze.md`
- Workflow کامل: `ponisha-trigger.md` · `AGENTS.md`
- تحلیل (فقط **استفاده** — نه توسعه): فایل‌های `config/*-analysis.md`
