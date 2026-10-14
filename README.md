# bond — لاندنج بيدج العيادات

صفحة هبوط ستاتيك لخدمات bond للدكاترة والمراكز الطبية.

## الملفات
```
index.html        الصفحة الرئيسية (VSL + أعمال + آراء + تصميمات + فورم)
thank-you.html    صفحة الشكر — بتفتح واتساب برسالة جاهزة
_headers          إعدادات الكاش (Cloudflare Pages)
assets/designs/   تصميمات لعملاء طبيين
assets/results/   صور قبل/بعد للأداء
```

## قبل النشر
في `index.html`:
- `SHEET_ENDPOINT` — لينك Apps Script اللي بيسجّل الليدز في Google Sheet (لسه فاضي)
- `BOND_WHATSAPP` — رقم الواتساب (بصيغة دولية من غير +)

## النشر
ستاتيك بالكامل — مفيش build step.
- **Vercel:** Framework = Other، وسيب Build/Output فاضيين
- **Cloudflare Pages:** ارفع الفولدر كله زي ما هو

## التتبّع
Meta Pixel + TikTok Pixel + GA4 — بيتحمّلوا بعد ما الصفحة تخلص رسم.
الأحداث: `contact` · `generate_lead` · `view_work` · `play_vsl` · `unqualified_lead`
