# تشغيل العارض الأرشيفي

هذه لقطات تاريخية أعيد بناؤها، وليست إصدارات مستقرة معتمدة. اختر المرحلة 06 للميزات الأوسع، أو المرحلة المطلوبة للمقارنة. نزّل أرشيف المصدر من الإصدار وفكّه، ثم افتح HTML المحدد أدناه. صفحة الملف في GitHub تعرض الشفرة ولا تشغّل العارض.

| المرحلة | ملف التشغيل | الإصدار | المصدر |
|---|---|---|---|
| 01 | `docs-viewer.html` | [الإصدار](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-01-base-reader) | [المصدر الثابت](https://github.com/Osama-Development/nes-markdown-viewer/blob/51029fa737b89f083be7618fd5f5b1f2264a616c/docs-viewer.html) |
| 02 | `docs-viewer-recording.html` | [الإصدار](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-02-recording-layout) | [المصدر الثابت](https://github.com/Osama-Development/nes-markdown-viewer/blob/84923098a848d9fc80d1c7efb45804337a306151/docs-viewer-recording.html) |
| 03 | `docs-viewer (1).html` | [الإصدار](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-03-collapsible-editor) | [المصدر الثابت](https://github.com/Osama-Development/nes-markdown-viewer/blob/2fbd1279b64110af2908553a8cf6e63ad69fced8/docs-viewer%20%281%29.html) |
| 04 | `NES_EDU_Markdown_Viewer_Final.html` | [الإصدار](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-04-source-drafts) | [المصدر الثابت](https://github.com/Osama-Development/nes-markdown-viewer/blob/5f77e90f329f09091ac524888d16c5b4d7b04470/NES_EDU_Markdown_Viewer_Final.html) |
| 05 | `NES_EDU_Markdown_Viewer_Visual_Edit_Final.html` | [الإصدار](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-05-visual-source-editor) | [المصدر الثابت](https://github.com/Osama-Development/nes-markdown-viewer/blob/fddcad3101b54255b78600541e74d32861ec9403/NES_EDU_Markdown_Viewer_Visual_Edit_Final.html) |
| 06 | `NES_EDU_Markdown_Viewer_Complete_Final.html` | [الإصدار](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-06-structural-editor) | [المصدر الثابت](https://github.com/Osama-Development/nes-markdown-viewer/blob/c09826fd1f50cd00cbd3accaf95d128152ca7847/NES_EDU_Markdown_Viewer_Complete_Final.html) |

## فتح مستند

1. افتح HTML بمتصفح حديث، ثم استخدم اختيار الملف أو ربط المجلد لتحميل Markdown موثوق بصيغة `.md` أو `.markdown` أو `.txt`.
2. مستندات المنهج المشار إليها في سجل العارض غير مرفقة باللقطات الست. اختر مستندك المحلي إذا طُلب ملف مفقود.
3. للتحميل النسبي ضع المستندات بجوار HTML، وافتح طرفية في المجلد وشغّل `python3 -m http.server 8000 --bind 127.0.0.1`. افتح `http://127.0.0.1:8000/` وانقر اسم HTML. أوقف الخادم بـ `Ctrl+C`. قد تمنع سياسات `file://` التحميل النسبي، مع بقاء منتقي الملفات خيارًا عمليًا.
4. الخطوط والأيقونات خارجية وتحتاج اتصالًا. المراحل 01–03 تحمل Marked من CDN غير مثبت الإصدار؛ المراحل 04–06 تتضمن المحلل داخل HTML.

## التحرير والتنزيل

المراحل 01–02 للعرض. المرحلة 03 تسمح بتحرير DOM وتعيد بناء Markdown من النص المعروض عند التصدير؛ قد تفقد التنسيق والروابط والجداول وبنية القوائم. احتفظ بالأصل وقارن التنزيل.

المرحلة 04 تضيف تحرير مصدر المقاطع/الملف ومسودات لكل مستند. المرحلة 05 تضيف تحريرًا مرئيًا مرتبطًا بالمصدر. المرحلة 06 تضيف عمليات البطاقات والعناوين والفواصل والبيانات الوصفية واختيار اسم التنزيل. ربط المقاطع بالمصدر تقريبي؛ اختبر النتيجة يدويًا على مستندك المركب.

في المراحل 04–06، المسودات نص صريح في `localStorage` داخل المتصفح. «محفوظ في المتصفح» لا تعني كتابة الملف الأصلي على القرص. نزّل Markdown وقارنه واحتفظ بنسخة مستقلة قبل مسح بيانات الموقع أو تبديل المتصفح/الأصل. إذا تعذر التخزين المحلي، نزّل التعديلات قبل الإغلاق. عند فقد المسودة ارجع إلى الأصل أو آخر تنزيل؛ لا توجد خدمة نسخ احتياطي أو مزامنة مرفقة.

## حدود التحقق

استخدم Markdown موثوقًا فقط؛ يُدرج ناتج Marked عبر `innerHTML` بلا تعقيم شامل. تسمية «تحرير آمن» في عنوان المصدر لا تعني تدقيقًا أمنيًا. السلوك التاريخي محفوظ كما هو.

طابقت المصادر SHA-256 في خطة الإصدارات وبايتات استجابات الوسوم المحفوظة. سجل سابق يثبت فحوص صياغة JavaScript فقط. لم تُجرَ اختبارات تشغيل متصفح أو يُثبت round-trip لتصدير Markdown. إشعار MIT المرفق خاص بـMarked ولا يمنح ترخيصًا جديدًا للتطبيق؛ الإصدار الدقيق للمحلل المضمن غير مثبت.

للتنقل داخل الشفرة استخدم `FUNCTION_LINE_INDEX.json` ثم رابط `line_url`. الروابط مثبتة إلى commit الاستعادة وأرقامها تخص HTML الأصلي. لا يشمل الفهرس دوال Marked أو callbacks المجهولة أو arrow functions أو الإغلاقات المحلية المتداخلة.
