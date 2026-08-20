# حافظه پیشنهادنویسی پونیشا

**قبل از نوشتن هر پیشنهاد این فایل را بخوان.** منبع اصلی علاقمندی‌ها و تأییدیه‌های من است.

---

## هدف سیستم (تأییدشده — Architect)

**Proposal Intelligence Engine** — افزایش Win Rate + **یادگیری مستمر** از نتایج واقعی.

متن زیبا که انتخاب را بالا نبرد = شکست.

| فایل | نقش |
|------|-----|
| `config/proposal-engine.md` | موتور: Risk، Insight، Client Simulation |
| `config/personal-voice.md` | شخصیت نوشتاری ثابت |
| `config/proposal-learning.md` | یادگیری از برد/باخت + Human Review |
| `config/negotiation-conversion-analysis.md` | **تحلیل funnel مذاکره → قرارداد** (Learning فقط) |
| `config/proposal-generation-logic-analysis.md` | **تحلیل منطق ساخت Proposal** (Learning فقط) |
| `config/project-selection-decision-analysis.md` | **تحلیل تصمیم انتخاب پروژه** — قبل از bid (Learning فقط) |
| `config/emotional-trust-layer-analysis.md` | **لایه اعتماد انسانی** — معیار کیفیت Proposal (Engine بدون تغییر) |
| `config/human-review-loop.md` | بازخورد ساخت‌یافته قبل از نسخه نهایی |
| `config/architecture-freeze.md` | **Stable** — شرایط تغییر معماری |

---

## ترتیب خواندن (یکپارچه — بدون تعارض)

| مرحله | فایل |
|-------|------|
| ۰ | `config/feasibility-check.md` |
| ۰.۵ | `config/project-selection-decision-analysis.md` — **قبل از Proposal** (هر «پونیشا»/«بعدی») |
| ۱ | این فایل (`MEMORY.md`) |
| ۲ | `config/proposal-learning.md` — Lessonهای دسته مرتبط |
| ۲.۵ | `config/proposal-generation-logic-analysis.md` — اگر پروژه Negotiation/Won/Lost |
| ۲.۶ | `config/negotiation-conversion-analysis.md` — اگر پاسخ کارفرما / مذاکره |
| ۳ | `config/personal-voice.md` |
| ۴ | `config/proposal-engine.md` — Risk + Insight + Simulation |
| ۵ | `config/profile-refresh.md` → `config/profile.md` |
| ۶ | `config/bids-log.md` |
| ۶.۵ | **`config/pending-bid-check.md`** — قبل از «پونیشا»/«بعدی» |
| ۶.۶ | **`config/last-proposal.md`** — بعد از هر Proposal به‌روز |
| ۷ | بودجه + `competition-guide.md` + `pricing-guide.md` |
| ۸ | `output-format.md` + `milestones-guide.md` |
| ۹ | `examples/winrate-*.txt` |
| ۱۰ | بعد از پیش‌نویس: `human-review-loop.md` + **`emotional-trust-layer-analysis.md`** |

---

## Architecture Freeze (Stable)

از ۱۴۰۵/۰۵/۱۵ سیستم **Stable** است. `config/architecture-freeze.md`

**تا رفع Freeze:** فقط Proposal، Human Review، Lesson، به‌روزرسانی داده learning.

**تغییر معماری** فایل‌های منجمد → یادآوری Freeze + سؤال: «آیا با وجود Freeze همچنان می‌خواهید معماری تغییر کند؟»

---

کاربر با **Cursor + AI** پروژه انجام می‌دهد. **قبل از پیشنهاد کارفرما** به خود کاربر بگو:

1. آیا با Cursor قابل انجام است؟
2. ریسک کم / متوسط / بالا؟
3. تناسب پروفایل، احتمال برد، رقابت، بودجه؟
4. **فعالیت کارفرما** — اگر بیش از ۷ روز بدون ورود/پاسخ/انتخاب/تعامل → اولویت پایین؛ قبل از Proposal: «سیگنال فعالیت کارفرما پایین است؛ پیشنهاد دادن احتمالاً ارزش زمان ندارد.» (حذف قطعی نیست — استثنا: Odoo/ERP/محصول آماده)
5. خارج از توان یا ریسک بالا -> **پیشنهاد ننویس** مگر کاربر بخواهد

جزئیات: `config/feasibility-check.md` — Skip و گزارش: `config/project-status.md`

**اگر قابل انجام است:** مرحله ۰ (ارزیابی) + **متن پیشنهاد + فرم پونیشا**

**در پیشنهاد کارفرما:** هرگز AI/Cursor/هوش مصنوعی ذکر نشود.

---

## لحن (تأییدشده)

طبق `config/personal-voice.md` — کوتاه، شفاف، مستقیم، مشاورمحور، فنی، آرام، بدون فروشندگی.

## چیزهایی که دوست ندارم (رد شده)

- پیشنهاد بلند با جدول، بولت زیاد، عنوان‌های رسمی
- لحن ربات/AI: «لطفاً توجه فرمایید»، «در خدمت شما»، «با احترام»، «خوشحال می‌شوم»
- فلش یونیکد `→` — فقط `->` یا شماره
- Lorem Ipsum و قول‌های توخالی
- **عدد زمان یا مبلغ داخل متن پیشنهاد**
- جملات کلیشه اعتمادسازی (لیست کامل: `proposal-engine.md`)
- شروع یکسان همه پیشنهادها با یک قالب ثابت
- اختراع تجربه/پروژه/مشتری/عدد/موفقیت (`proposal-engine.md`)

## ساختار خروجی (تأییدشده — همیشه دو بلوک)

**هر پیشنهاد بدون استثنا دو قسمت جدا:**

### بلوک ۱ — متن پیشنهاد

برای کپی در چت پونیشا. طبق `proposal-engine.md` + `personal-voice.md`:

- Risk Discovery: یک ریسک **مخصوص این پروژه**
- Insight: یک نکته واقعی — یا هیچ (مصنوعی ممنوع)
- Client Simulation: «آیا کارفرما حداقل یک پیام می‌فرستاد؟»
- ۴–۸ جمله؛ حداکثر ~۱۲ خط

**ممنوع در متن پیشنهاد:** هر عدد زمان یا قیمت.

### بلوک ۲ — فرم پونیشا
فرمت 📋 — `config/output-format.md` — هر فیلد code block جدا.

**مرحله ۰:** حتماً لینک `https://ponisha.ir/project/{ID}` — جزئیات: `output-format.md`

زمان تحویل و مبلغ کل هر کدام خط جدا. هر مرحله: عنوان فارسی کوتاه + خط بعد «مبلغ: X تومان». بدون FA+EN در یک خط.

جزئیات: `config/output-format.md` — نمونه Win Rate: `examples/winrate-*.txt`

## وقتی گفت «کوتاه‌تر / صمیمی‌تر / فنی»

نسخه قبلی را خلاصه کن؛ محتوا حفظ، طول کمتر. الگو: `examples/engineering-company-short.txt`

## مراحل + قیمت (تأییدشده)

همیشه داخل **بلوک ۲**:

- زمان تحویل کل
- مبلغ کل
- ۳ یا ۴ مرحله؛ جمع = مبلغ کل

جزئیات: `config/milestones-guide.md`

## قیمت‌گذاری (اصول — بدون تغییر)

- **قانون اجباری:** مبلغ فرم **داخل بازه بودجه پروژه**
- **جایگاه:** معمولاً **میانه بازه** (مثال: ۷۴۸۸۵۰، بودجه ۲۰–۴۵M → ۳۰M)
- اگر بازه نبود → `pricing-guide.md` + رقابت
- scope مبهم: قیمت اولیه داخل بازه + «بعد از جزئیات تنظیم می‌کنم» (در متن، بدون عدد)

## الگوهای فنی تأییدشده

**سایت HTML اختصاصی:** HTML/CSS/JS، ریسپانسیو، اسکلت/UI اول.

**وردپرس پاک‌سازی:** بکاپ، آپدیت، DB، cPanel، امنیت، ۷ روز پشتیبانی.

**وردپرس + Elementor:** Hello Elementor + Pro، بدون دمو. GTmetrix، فونت لوکال.

**سایت شرکتی فنی:** wireframe -> UI -> کد -> تست.

**nopCommerce:** مقایسه مرجع، Razor/CSS/JS، IIS.

**ماژول پنل:** دسته‌بندی + خروجی per دسته.

## نمونه‌ها

| نوع | فایل |
|-----|------|
| **Win Rate (جدید — الگوی اصلی)** | `examples/winrate-*.txt` |
| فرمت دو بلوک کلاسیک | `examples/woocommerce-sections.txt` |
| وردپرس پاک‌سازی | `examples/wordpress-cleanup.txt` |
| ووکامرس / nopCommerce / … | `examples/` |

## workflow برای agent

**تریگر «پونیشا» / «بعدی» بدون متن آگهی:** `config/ponisha-trigger.md` — **هرگز** متن پروژه نخواه.

0. **`pending-bid-check.md`** — قبل از جستجو
1. **`feasibility-check.md`** — اگر نه/ریسک بالا → توقف
1.۵ **`project-selection-decision-analysis.md`** — دلیل انتخاب + امتیاز + گزینه رد
2. `MEMORY.md` + `proposal-learning.md` + `personal-voice.md` + `proposal-engine.md`
3. پروفایل: `profile-refresh.md` — هر **۷ روز**
4. جستجو در ponisha.ir — Fit اول، Freshness، HTML «انتخاب کرده»
5. `bids-log.md` — Skip + رد شده
6. Risk → Insight → بلوk ۱ → Simulation → **Emotional Trust Layer** → بلوk ۲ (📋)
7. **مرحله ۰** با **لینک** + **`last-proposal.md`**
8. **Human Review Loop** (+ ارتباط انسانی ⭐)

**تریگرها:**

| عبارت | عمل |
|--------|-----|
| «پونیشا» / «بعدی» | Pending Bid Check → trigger → **Selection Analysis** → جستجو |
| «پیشنهاد دادم» | bids-log + learning + last-proposal → Submitted + **Logic Analysis (بخش ۱–۳)** |
| «پاسخ داد» / مذاکره | Negotiation Engine + **Conversion Analysis** + Logic Analysis (بخش ۴) |
| «بردیم» / «باختیم» | learning + **Conversion (#5)** + **Logic (بخش ۴–۵)** |
| «خوبه» | Ready |

## به‌روزرسانی

- اصول Intelligence → `proposal-engine.md` / `proposal-learning.md` / `personal-voice.md` / `human-review-loop.md`
- پروفایل → هر ۷ روز → `profile.md`
