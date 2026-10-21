# Sehhati (صحتي) — Potassium Bromate Checker

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23532157.svg)](https://doi.org/10.5281/zenodo.23532157)

**Live app:** https://sehhati-sd.netlify.app

A free, mobile-first web app that helps consumers check bread and flour ingredient lists for **potassium bromate (E924)** and other flagged dough improvers, and guides them through lab testing and filing a complaint with the competent authority.

[العربية](#العربية)

---

## Why this project

Potassium bromate is a flour improver classified by IARC as Group 2B (possibly carcinogenic to humans) and banned in many countries. In many markets, bread is sold without an ingredient label, and consumers have no simple way to check. Sehhati turns that into a one-minute check and a clear next step.

## Features

- **Ingredient scan:** paste an ingredient list; the app detects potassium bromate under its different names and codes (Arabic and English, E924 / E924b), plus azodicarbonamide (E927a) and potassium iodate (E917) as extra warnings.
- **Barcode lookup:** type or scan a barcode (camera, on supported browsers); ingredients are fetched from [Open Food Facts](https://world.openfoodfacts.org) and checked.
- **Flour and bakery registry:** searchable results of documented lab analyses (`data.json`).
- **Complaint generator:** builds a ready-to-send complaint letter (copy or share via WhatsApp). Nothing is stored or sent by the app.
- **Guide:** questions to ask the bakery, how to take a sample for lab analysis, and buying tips.
- **Private history:** recent checks are kept in the browser's `localStorage` on the user's device only.
- **Installable PWA:** manifest and service worker, RTL Arabic UI, light/dark themes.

## Tech

Plain HTML, CSS and JavaScript. No framework, no backend, no API keys. Hosted on Netlify.

| File | Purpose |
|---|---|
| `index.html` | App UI and detection logic |
| `data.json` | Flour and bakery lab-results registry |
| `manifest.webmanifest`, `sw.js`, `icon-192.png` | PWA support |

## Privacy

All checks run in the browser. The only external request is the optional barcode lookup, which sends the barcode number to Open Food Facts. No accounts, no tracking.

## Disclaimer

The app reads only the text the user enters. Confirming the presence of potassium bromate requires **laboratory analysis**. Results are informational and not legal or medical advice.

Registry data is compiled from published laboratory reports and reflects only the samples analyzed in those reports; it does not describe any product or bakery as a whole, and it may not reflect current production.

## Citation

Suliman, E. D. (2026). *Sehhati (صحتي): A Web App for Detecting Potassium Bromate (E924) in Bread and Flour Ingredient Lists* (Version v1.0) [Computer software]. Zenodo. https://doi.org/10.5281/zenodo.23532157

## Author and rights

**Elnazeer Dawod Suliman Abdalla** — MACKENZIE Center for Computing, Training & Consulting, Republic of the Sudan.

Registered work, certificate no. 20562/أ/2021م 21 ت, issued 15 September 2021 by the Copyright and Neighbouring Rights Council.

© 2021–2026 Elnazeer Dawod Suliman. **All rights reserved.** No permission is granted to copy, modify or redistribute this code without written consent.

Patents and other work: https://www.linkedin.com/in/elnazeer-dawod-suliman-4b0201358/

---

<a id="العربية"></a>

<div dir="rtl">

# صحتي — كاشف برومات البوتاسيوم

**التطبيق المباشر:** https://sehhati-sd.netlify.app

تطبيق ويب مجاني مصمم للهاتف يساعد المستهلك على فحص قوائم مكونات الخبز والدقيق للكشف عن **برومات البوتاسيوم (E924)** وغيرها من محسّنات العجين المقيّدة، ويرشده إلى التحليل المخبري وتقديم الشكوى للجهة المختصة.

## لماذا هذا المشروع

صنّفت الوكالة الدولية لأبحاث السرطان برومات البوتاسيوم ضمن المجموعة 2B (ربما مسرطنة للإنسان)، وهي محظورة في دول كثيرة. وفي أسواق كثيرة يُباع الخبز بلا قائمة مكونات، فلا يجد المستهلك وسيلة بسيطة للتحقق. «صحتي» تحوّل ذلك إلى فحص من دقيقة وخطوة تالية واضحة.

## المزايا

- **فحص المكونات:** الصق القائمة فيكشف التطبيق المادة بأسمائها ورموزها (عربي وإنجليزي، E924 وE924b)، ويُنبّه إلى الأزوديكربوناميد (E927a) ويودات البوتاسيوم (E917).
- **البحث بالباركود:** اكتب الرقم أو امسحه بالكاميرا (في المتصفحات الداعمة)، فتُجلب المكونات من Open Food Facts وتُفحص.
- **سجل الدقيق والمخابز:** نتائج تحاليل مخبرية موثّقة قابلة للبحث (`data.json`).
- **مولّد الشكوى:** ينشئ نص شكوى جاهزاً للنسخ أو الإرسال عبر واتساب، ولا يحفظ التطبيق شيئاً ولا يرسله.
- **الدليل:** أسئلة للمخبز، وطريقة أخذ عينة للتحليل، ونصائح الشراء.
- **سجل خاص:** آخر الفحوصات محفوظة في متصفحك على جهازك فقط.
- **تطبيق قابل للتثبيت (PWA)** بواجهة عربية من اليمين لليسار ووضعين فاتح وداكن.

## التقنيات

HTML وCSS وJavaScript خام، بلا إطار عمل ولا خادم ولا مفاتيح API، ومستضاف على Netlify.

## الخصوصية

كل الفحوصات تعمل داخل المتصفح. الطلب الخارجي الوحيد هو البحث بالباركود (اختياري) ويرسل رقم الباركود فقط إلى Open Food Facts. لا حسابات ولا تتبع.

## تنبيه

يقرأ التطبيق النص الذي يدخله المستخدم فقط. والتأكد من وجود برومات البوتاسيوم يتطلب **تحليلاً مخبرياً**. النتائج إرشادية وليست مشورة قانونية أو طبية.

بيانات السجل مجمّعة من تقارير مخبرية منشورة، وتخص العينات المحلَّلة في تلك التقارير فقط، ولا تصف المنتج أو المخبز ككل، وقد لا تعكس الإنتاج الحالي.

## الاستشهاد

Suliman, E. D. (2026). Sehhati (صحتي): A Web App for Detecting Potassium Bromate (E924) in Bread and Flour Ingredient Lists (Version v1.0) [Computer software]. Zenodo. https://doi.org/10.5281/zenodo.23532157

## المؤلف والحقوق

**النذير داود سليمان عبدالله** — مركز MACKENZIE للحوسبة والتدريب والاستشارات، جمهورية السودان.

مصنف مسجّل برقم 20562/أ/2021م 21 ت، صدرت شهادته في 15 سبتمبر 2021م عن مجلس حق المؤلف والحقوق المجاورة.

© 2021–2026 النذير داود سليمان. **جميع الحقوق محفوظة.** لا يجوز نسخ الكود أو تعديله أو إعادة توزيعه دون إذن كتابي.

البراءات والأعمال الأخرى: https://www.linkedin.com/in/elnazeer-dawod-suliman-4b0201358/

</div>
