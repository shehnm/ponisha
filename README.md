# Ponisha — Proposal Intelligence Engine

سیستم پیشنهاد پونیشا با هدف **Win Rate** + **یادگیری مستمر**.

## شروع

1. workspace را اضافه کنید
2. Agent طبق `AGENTS.md` عمل می‌کند

## معماری

```
feasibility → learning (دسته) → personal-voice → proposal-engine
    → Risk Discovery → Insight → بلوک ۱ → Client Simulation → بلوک ۲
    → [بعد از نتیجه] proposal-learning
    → [بعد از هر پیش‌نویس] human-review-loop → نسخه نهایی
    → معماری: FROZEN (architecture-freeze.md)
```

## فایل‌های کلیدی

| فایل | نقش |
|------|-----|
| `AGENTS.md` | workflow |
| `MEMORY.md` | حافظه اصلی |
| **`config/proposal-engine.md`** | Risk، Insight، Client Simulation |
| **`config/personal-voice.md`** | شخصیت نوشتاری |
| **`config/human-review-loop.md`** | بازخورد ساخت‌یافته ۱–۵ قبل از نسخه نهایی |
| **`config/proposal-learning.md`** | یادگیری + System Metrics |
| **`config/architecture-freeze.md`** | **Stable** — شرایط تغییر معماری |
| `config/feasibility-check.md` | فیلتر قبل از bid |
| `config/output-format.md` | دو بلوک |
| `config/pricing-guide.md` | بودجه |
| `config/milestones-guide.md` | مراحل |
| `config/competition-guide.md` | رقابت |
| `config/bids-log.md` | لاگ سریع |
| `config/profile.md` | پروفایل |
| `examples/winrate-*.txt` | نمونه‌ها |

## ریپو

https://github.com/shehnm/ponisha
