# دستورالعمل Agent — Proposal Intelligence Engine

## ⚠️ Execution Mode — سیستم تحلیل کامل است

**«پونیشا» / «بعدی» = فقط اجرا** — `config/execution-mode.md`

- **نه** Layer / Rule / Engine / تحلیل جدید (مگر مشکل تکرارشونده از داده + Override)
- **تمرکز:** پروژه مناسب → Proposal → ثبت نتیجه → Validation
- هر Proposal: Copy/Paste · Decision Trace · بعد از outcome → Hypothesis Validation

---

## ⚠️ تریگر «پونیشا» / «بعدی» (اولین کار)

**اگر کاربر فقط گفت «پونیشا» یا «بعدی» (بدون متن آگهی):**

→ **`config/ponisha-trigger.md` را بخوان و اجرا کن.**  
→ **هرگز** نگو «متن آگهی پروژه را بفرست» — خودت پروژه را از پونیشا پیدا کن.

---

## Session Startup

**قبل از کار مرتبط با پونیشا / Proposal / مذاکره / پروژه جدید:** `config/session-startup-check.md` — Load قوانین از فایل ریپو؛ اولین پاسخ Session:

> قوانین پروژه پونیشا بررسی شد. نسخه فعلی Workflow فعال است.

---

## قبل از هر کار (ترتیب ثابت)

0. **`config/session-startup-check.md`**
1. **`config/pending-bid-check.md`** — قبل از «پونیشا» / «بعدی»
2. **`config/ponisha-trigger.md`** — اگر تریگر بدون متن آگهی
3. **`config/feasibility-check.md`**
3.۵ **`config/project-selection-decision-analysis.md`** — **قبل از Proposal**
3.۶ **`config/proposal-intent-control.md`** — **Stage Funnel + هدف پیام** — قبل از نوشتن بلوک ۱
4. **`MEMORY.md`**
5. **`config/proposal-learning.md`** + **`personal-voice.md`** + **`proposal-engine.md`**
5.۴ **`config/emotional-trust-layer-analysis.md`** — **قبل از Human Review** (معیار کیفیت روان‌شناسی — Engine بدون تغییر)
5.۴۵ **`proposal-engine.md` → Client Understanding Check** — **تست ۰ (۲ جمله اول) + ۵ سؤال** قبل HR؛ فنی درست ≠ کافی
5.۵ **`config/negotiation-conversion-analysis.md`** + **`config/proposal-generation-logic-analysis.md`** — هنگام مذاکره / پاسخ کارفرما / Won / Lost
6. **`config/bids-log.md`** — Skip + رد شده + تکرار ممنوع
7. پروفایل (sync ۷ روز): **`config/profile-refresh.md`**
8. **`config/output-format.md`** + pricing + competition + milestones
9. بعد از پیش‌نویس: **`human-review-loop.md`** + **`emotional-trust-layer-analysis.md`**

---

## خروجی

- **مرحله ۰:** ارزیابی — **حتماً** `#ID` + عنوان + **لینک** `https://ponisha.ir/project/{ID}` (`output-format.md`)
- **مرحله ۱:** بلوک ۱ + ۲ (📋 code blocks) — پیش‌نویس + به‌روز **`last-proposal.md`**
- **مرحله ۲:** Human Review Loop — چک‌لیست (۵ کلاسیک + ۵ روان‌شناسی)

---

## تریگرها

| عبارت | عمل |
|--------|-----|
| «پونیشا» / «بعدی» | Pending Bid Check → trigger → **Selection Analysis** → جستجو + پیشنهاد |
| «پیشنهاد دادم» | `bids-log` (+ متن) + `proposal-learning` + `last-proposal` → Submitted |
| «هنوز ارسال نکردم» | Ready بماند؛ پروژه جدید فقط با **تأیید صریح** |
| «خوبه» | `last-proposal` → Ready |
| «بردیم» / «باختیم» / «پاسخ داد» | تحلیل + Lesson + Conversion + Logic + Selection + **Hypothesis Validation** |

---

## هرگز

- از کاربر متن آگهی نخواه (مگر استثنا در `ponisha-trigger.md`)
- **مرحله ۰ بدون لینک پروژه**
- git merge / branch switch بدون درخواست کاربر
- web-fetch تصادفی بدون برنامه جستجو
- HTML «انتخاب کرده» را نادیده بگیر

---

## Architecture Freeze

قبل از تغییر معماری: **`config/architecture-freeze.md`**

## نام‌گذاری

در متن فارسی فقط **پونیشا** — **نه** «پونیش»+a لاتین، **نه** «بعد»+i لاتین.
URL (`ponisha.ir/project/...`) جدا و مجاز.

## commit

داده learning/bids/profile — مجاز. تغییر معماری منجمد — فقط Freeze یا Override.
