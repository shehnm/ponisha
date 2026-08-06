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
| `config/proposal-learning.md` | یادگیری از برد/باخت |

---

## ترتیب خواندن (یکپارچه — بدون تعارض)

| مرحله | فایل |
|-------|------|
| ۰ | `config/feasibility-check.md` |
| ۱ | این فایل (`MEMORY.md`) |
| ۲ | `config/proposal-learning.md` — Lessonهای دسته مرتبط |
| ۳ | `config/personal-voice.md` |
| ۴ | `config/proposal-engine.md` — Risk + Insight + Simulation |
| ۵ | `config/profile-refresh.md` → `config/profile.md` |
| ۶ | `config/bids-log.md` |
| ۷ | بودجه + `competition-guide.md` + `pricing-guide.md` |
| ۸ | `output-format.md` + `milestones-guide.md` |
| ۹ | `examples/winrate-*.txt` |

---

## ارزیابی قبل از پیشنهاد (اجباری)

کاربر با **Cursor + AI** پروژه انجام می‌دهد. **قبل از پیشنهاد کارفرما** به خود کاربر بگو:

1. آیا با Cursor قابل انجام است؟
2. ریسک کم / متوسط / بالا؟
3. خارج از توان یا ریسک بالا -> **پیشنهاد ننویس** مگر کاربر بخواهد

جزئیات: `config/feasibility-check.md`

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

```
زمان تحویل: ...
مبلغ کل: ...

مرحله ۱ — عنوان — مبلغ
مرحله ۲ — ...
```

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

0. `feasibility-check.md` — اگر نه/ریسک بالا → توقف
1. `MEMORY.md` + `proposal-learning.md` (دسته مرتبط) + `personal-voice.md` + `proposal-engine.md`
2. پروفایل: `profile-refresh.md` — هر **۷ روز**
3. brief یا جستجو («پونیشا» / «بعدی»)
4. `bids-log.md` — تکرار نکن
5. بودجه + رقابت
6. Risk Discovery → Insight → بلوک ۱ → Client Simulation → امتیازدهی
7. خروجی دو بلوکی

**تریگرها:**

| عبارت | عمل |
|--------|-----|
| «پیشنهاد دادم» | `bids-log.md` + ردیف اولیه `proposal-learning.md` |
| «بردیم» / «باختیم» / «پاسخ داد» | تحلیل + Lesson در `proposal-learning.md` |

## به‌روزرسانی

- اصول Intelligence → `proposal-engine.md` / `proposal-learning.md` / `personal-voice.md`
- پروفایل → هر ۷ روز → `profile.md`
