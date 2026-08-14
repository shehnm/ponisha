# پونیشا — حافظه پیشنهادنویسی

تنظیمات، سبک و نمونه پیشنهادهای **پونیشا** برای Cursor.

**Life OS:** [README-LIFE-OS.md](./README-LIFE-OS.md) · مدیریت: [AGENTS-LIFE-OS.md](./AGENTS-LIFE-OS.md)  

**نام‌گذاری:** در متن فارسی فقط «پونیشا» — جزئیات: `config/output-format.md`

---

## وقتی گفت «پونیشا» یا «بعدی»

**این ریپو برای همین ساخته شده.** Agent نباید بپرسد «متن آگهی را بفرست».

1. **`config/ponisha-trigger.md`** ← **شروع از اینجا**
2. **`config/session-startup-check.md`** — Load قوانین
3. خودت پروژه باز را از `ponisha.ir` پیدا کن
4. `config/bids-log.md` + HTML «انتخاب کرده» را چک کن
5. مرحله ۰ (ارزیابی) + مرحله ۱ (پیشنهاد Copy-Friendly)

---

## شروع

1. این پوشه را به workspace اضافه کنید
2. **`config/session-startup-check.md`** — قبل از «پونیشا» / Proposal، قوانین را از فایل Load کنید
3. Agent قبل از هر پیشنهاد `MEMORY.md` را می‌خواند

## فایل‌های مهم

| فایل | نقش |
|------|-----|
| **`config/ponisha-trigger.md`** | **تریگر «پونیشا»** — Decision Tree + ممنوعات |
| `config/session-startup-check.md` | **Startup Check** — Load قوانین Session |
| `MEMORY.md` | **حافظه اصلی** — لحن، تأییدیه‌ها، workflow |
| `AGENTS.md` | دستورالعمل agent |
| `.cursor/rules/` | قانون alwaysApply در Cursor |
| `config/bids-log.md` | لاگ bid + Skip + رد شده |
| `config/project-status.md` | وضعیت پروژه‌ها + صف اسکن |
| `config/pricing-guide.md` | بازه قیمت پروژه‌ها |
| `config/output-format.md` | فرمت دو بلوکی تأییدشده |
| `config/profile.md` | داده پروفایل shehneh |
| `config/feasibility-check.md` | **Project Selection + Feasibility** (Freshness، فعالیت کارفرما) |
| `config/profile-refresh.md` | بازه ۷ روزه sync پروفایل |
| `config/competition-guide.md` | رقابت هر پروژه (از اسکرین) |
| `examples/` | پیشنهادهای تأییدشده |

## ریپو

https://github.com/shehnm/ponisha
