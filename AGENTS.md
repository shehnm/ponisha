# دستورالعمل Agent — Proposal Intelligence Engine

## هدف

افزایش **Win Rate** + **یادگیری مستمر** از نتایج واقعی.

## قبل از هر کار (ترتیب ثابت)

0. **`config/feasibility-check.md`**
1. **`MEMORY.md`**
2. **`config/proposal-learning.md`** — Lessonهای دسته مرتبط
3. **`config/personal-voice.md`**
4. **`config/proposal-engine.md`** — Risk + Insight + Client Simulation
5. **`config/profile-refresh.md`** (۷ روز)
6. **`config/bids-log.md`**
7. بودجه + **`pricing-guide.md`** + **`competition-guide.md`**
8. **`output-format.md`** + **`milestones-guide.md`**

**قبل از «پونیشا» / «بعدی»:** **`config/pending-bid-check.md`** — اگر last-proposal در bids-log نیست → توقف و سؤال از کاربر (پروژه جدید نساز).

## خروجی

- **مرحله ۰:** ارزیابی feasibility
- **مرحله ۱:** بلوک ۱ + بلوک ۲ (**پیش‌نویس**)
- **مرحله ۲:** Human Review Loop (`human-review-loop.md`) — چک‌لیست ۱–۵
- **نسخه نهایی:** بعد از Review یا «خوبه» بدون اصلاح

## تریگرها

| عبارت | عمل |
|--------|-----|
| «پونیشا» / «بعدی» | **Pending Bid Check** → سپس جستجو + پیشنهاد؛ **`config/last-proposal.md`** را بعد از هر Proposal به‌روز کن |
| «پیشنهاد دادم» | `bids-log` (+ متن Proposal) + ردیف اولیه `proposal-learning` + `last-proposal` → Submitted |
| «هنوز ارسال نکردم» | بدون تغییر bids-log؛ پروژه جدید شروع نشود |
| «بردیم» | تحلیل پیروزی + Lesson |
| «باختیم» | تحلیل شکست + Lesson |
| «پاسخ داد» | آپدیت `proposal-learning` |
| بازخورد Human Review | Lesson `[Human]`؛ تکرار ≥۳ → پیشنهاد اصلاح Engine |

## Architecture Freeze

قبل از تغییر معماری فایل‌های منجمد: **`config/architecture-freeze.md`**

- Stable از ۱۴۰۵/۰۵/۱۵
- نیاز: ۲۰ Proposal + ۱۰ نتیجه + مشکل تکرارشونده — **یا** تأیید صریح کاربر پس از یادآوری

## commit

داده learning/bids/profile — مجاز. تغییر معماری منجمد — فقط Freeze یا Override.
