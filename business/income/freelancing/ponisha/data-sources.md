# منابع داده — گزارش پونیشا

**تاریخ snapshot:** ۱۴۰۵/۰۵/۲۱ (v1.1 — اصلاح Won)  
**قانون:** بدون فرض — فقط آنچه در فایل یا لاگ ثبت شده.

## منابع استفاده‌شده

| منبع | مسیر (ریپو ponisha) | آخرین به‌روزرسانی در snapshot |
|------|---------------------|-------------------------------|
| لاگ پیشنهادها | `config/bids-log.md` | ۱۴۰۵/۰۵/۲۱ |
| Won تاریخی | `config/won-log.md` | ۱۴۰۵/۰۵/۲۱ |
| Won Pattern (تحلیل) | `business/income/freelancing/ponisha/won-patterns/` | ۱۴۰۵/۰۵/۲۱ |
| گزارش روزانه | `daily-management-report-1405-05-21.md` | ۱۴۰۵/۰۵/۲۱ |
| پروفایل | `config/profile.md` | ۱۴۰۵/۰۵/۲۰ |
| وضعیت پروژه / Fresh bids | `config/project-status.md` | ۱۴۰۵/۰۵/۲۱ |
| انتخاب پروژه / Feasibility | `config/feasibility-check.md` | ثابت (policy) |
| حافظه تأییدشده | `MEMORY.md` | ثابت (workflow) |
| راهنمای رقابت | `config/competition-guide.md` | ثابت |
| راهنمای قیمت | `config/pricing-guide.md` | ثابت |

## منابع **موجود نیست** (در branch فعلی)

| فایل | وضعیت |
|------|--------|
| `config/proposal-engine.md` | **نیست** — branch `cursor/proposal-engine-winrate-40a7` |
| `config/human-review-loop.md` | **نیست** |
| `config/pending-bid-check.md` | **نیست** |
| `config/architecture-freeze.md` | **نیست** |
| Won/Lost کامل campaign | **ناقص** — ۱ Lost در bids-log؛ ۲۲ Submitted باز |
| Won تاریخی (قبل از campaign) | ✅ `config/won-log.md` — **۴ Won** |
| درآمد واقعی Won | **۶۳,۲۰۰,۰۰۰** تومان (مبلغ توافق نهایی) |

## محدودیت‌ها

1. **Win Rate campaign** فقط از ردیف‌های Won/Lost در `bids-log` — Won تاریخی در `won-log.md` جداست.
2. **Win Rate ترکیبی** = won-log (۴) + Lost campaign (۱) = **۸۰٪** — v1.0 گزارش ۰٪ بود چون won-log نبود.
3. **تحلیل انتخاب پروژه** در گفتگوها تا وقتی در `bids-log` (Skip/رد شده) ثبت نشود، در گزارش نیامده.
4. **مبلغ Won:** معیار تحلیل = **مبلغ توافق نهایی** — نه بازه بودجه صفحه.
5. **مبلغ/زمان bid** از اعلام کاربر («پیشنهاد دادم») — اگر با فرم پونیشا فرق داشت، باید دستی اصلاح شود.
