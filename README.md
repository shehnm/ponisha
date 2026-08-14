# پونیشا — حافظه پیشنهادنویسی + Proposal Intelligence

تنظیمات، سبک، workflow و نمونه پیشنهادهای **پونیشا** برای Cursor.

**Life OS:** [README-LIFE-OS.md](./README-LIFE-OS.md) · مدیریت: [AGENTS-LIFE-OS.md](./AGENTS-LIFE-OS.md)

---

## وقتی گفت «پونیشا» یا «بعدی»

Agent **نباید** بپرسد «متن آگهی را بفرست».

1. **`config/ponisha-trigger.md`** ← شروع
2. **`config/session-startup-check.md`** — Load قوانین
3. **`config/pending-bid-check.md`** — چک Ready
4. خودت پروژه باز را از `ponisha.ir` پیدا کن
5. **مرحله ۰** با **لینک** + **مرحله ۱** با 📋 code blocks

---

## معماری

```
feasibility → learning → voice → proposal-engine
    → Risk → Insight → بلوک ۱ → Simulation → بلوک ۲ (📋)
    → human-review-loop → last-proposal.md
```

## فایل‌های کلیدی

| فایل | نقش |
|------|-----|
| **`config/ponisha-trigger.md`** | تریگر — خودت پروژه پیدا کن |
| **`config/session-startup-check.md`** | Startup Check |
| **`config/pending-bid-check.md`** | Ready vs Submitted |
| **`config/last-proposal.md`** | آخرین پیش‌نویس + **لینک** |
| **`config/output-format.md`** | 📋 کپی + **لینک اجباری مرحله ۰** |
| `AGENTS.md` | workflow |
| `MEMORY.md` | حافظه اصلی |
| `config/proposal-engine.md` | Risk، Insight، Simulation |
| `config/human-review-loop.md` | Human Review |
| `config/bids-log.md` | لاگ bid + Skip |
| `config/project-status.md` | وضعیت + صف اسکن |
| `examples/winrate-*.txt` | نمونه Win Rate |

## ریپو

https://github.com/shehnm/ponisha
