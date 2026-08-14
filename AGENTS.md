# دستورالعمل Agent — پیشنهاد پونیشا

## ⚠️ تریگر «پونیشا» / «بعدی» (اولین کار)

**اگر کاربر فقط گفت «پونیشا» یا «بعدی» (بدون متن آگهی):**

→ **`config/ponisha-trigger.md` را بخوان و اجرا کن.**  
→ **هرگز** نگو «متن آگهی پروژه را بفرست» — خودت پروژه را از پونیشا پیدا کن.

---

## Session Startup

**قبل از کار مرتبط با پونیشا / Proposal / مذاکره / پروژه جدید:** `config/session-startup-check.md` — Load قوانین از فایل ریپو؛ اولین پاسخ Session یک خط تأیید.

## قبل از هر کار

0. **`config/session-startup-check.md`** — Session تازه یا تریگر workflow پونیشا
1. **`config/ponisha-trigger.md`** — اگر تریگر «پونیشا» / «بعدی»
2. **`config/feasibility-check.md`** — ارزیابی + Fresh Project Priority + فعالیت کارفرما؛ اگر ریسک بالا/غیرممکن -> پیشنهاد نده
3. **`MEMORY.md`**
4. **`config/bids-log.md`** — Skip + رد شده + تکرار ممنوع
5. پروفایل (sync ۷ روز): `config/profile-refresh.md`
6. **`config/output-format.md`**
7. رقبا (اسکرین): `config/competition-guide.md`

## خروجی

- **مرحله ۰:** ارزیابی (فقط به کاربر)
- **مرحله ۱ (اگر OK):** متن پیشنهاد + فرم پونیشا — **Copy-Friendly** (`output-format.md`)
- قبل از تحویل: Copy-Friendly + نام **«پونیشا»** (`output-format.md` — Naming Convention)
- «آیا با یک کلیک Copy و بدون اصلاح Paste می‌شود؟» — اگر نه، بازنویسی

## هرگز

- از کاربر متن آگهی نخواه (مگر ID بدون fetch یا همه کاندیدها رد شده)
- git merge / branch switch بدون درخواست کاربر
- web-fetch تصادفی بدون برنامه جستجوی پروژه
- HTML «انتخاب کرده» را نادیده بگیر

## نام‌گذاری

در متن فارسی فقط **پونیشا** — نه Ponisha، نه حرف لاتین داخل کلمه. URL و نام ریپو (`ponisha`) جدا از متن.

## commit

تنظیمات یا sync پروفایل — با درخواست یا تغییر معنادار.
