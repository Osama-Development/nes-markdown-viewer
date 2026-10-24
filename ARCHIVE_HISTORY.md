# تاريخ اللقطات المستعادة

الترتيب مبني على وقت إنشاء الملف المرصود في سجل المصدر، وليس تاريخ Git أصليًا مثبتًا. الإصدارات الستة مسجلة بأنها متحقق منها في `release_plan.json` الحالي؛ كلها prereleases أرشيفية أعيد بناؤها. لا تُستبدل أوقات المصدر بأوقات الاستعادة ولا تُنسب commits الاستعادة إلى المطور الأصلي.

كل حالة تضم HTML الأصلي المختار وحده مع وثائقها. انتقال اسم الملف بين الحالات تمثيل للاستعادة وليس دليلًا على rename تاريخي. commits التحضير المحلية منفصلة عن commits Work الموثقة بحساب المالك عن بُعد، ولا يُفترض تطابق SHA بينهما.

| المرحلة | وقت إنشاء المصدر المرصود (UTC) | الوسم | commit الاستعادة عن بُعد |
|---|---|---|---|
| 01 | 2026-10-21T17:00:52.039291Z | [archive-01-base-reader](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-01-base-reader) | `51029fa737b89f083be7618fd5f5b1f2264a616c` |
| 02 | 2026-10-21T17:12:16.139255Z | [archive-02-recording-layout](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-02-recording-layout) | `84923098a848d9fc80d1c7efb45804337a306151` |
| 03 | 2026-10-21T18:06:42.522824Z | [archive-03-collapsible-editor](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-03-collapsible-editor) | `2fbd1279b64110af2908553a8cf6e63ad69fced8` |
| 04 | 2026-10-21T18:27:34.406187Z | [archive-04-source-drafts](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-04-source-drafts) | `5f77e90f329f09091ac524888d16c5b4d7b04470` |
| 05 | 2026-10-21T18:55:51.226577Z | [archive-05-visual-source-editor](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-05-visual-source-editor) | `fddcad3101b54255b78600541e74d32861ec9403` |
| 06 | 2026-10-21T19:18:06.485316Z | [archive-06-structural-editor](https://github.com/Osama-Development/nes-markdown-viewer/releases/tag/archive-06-structural-editor) | `c09826fd1f50cd00cbd3accaf95d128152ca7847` |

## التغيرات المرصودة

- **01:** عارض RTL أساسي واختيار ملف/مجلد وفهرس عناوين وتنسيق إشارات الشرائح.
- **02:** تنسيق مخصص للإلقاء/التسجيل وإضافة مستند التسجيل إلى السجل.
- **03:** طي الرأس والفهرس والتنقل بلوحة المفاتيح وتصنيف النبرة والتحرير الأولي داخل DOM؛ قصور التصدير التاريخي محفوظ.
- **04:** تحرير قائم على المصدر ومسودات لكل مستند وتصدير المصدر وتضمين Marked.
- **05:** ربط النص المرئي بمواضع المصدر والتحرير بالنقر وحفظ المسودة المؤجل.
- **06:** عمليات بنية البطاقات والفقرات والعناوين والبيانات الوصفية وتحديد اسم التصدير.

## بصمات المصدر

| الملف | SHA-256 |
|---|---|
| `docs-viewer.html` | `1dccd4de3e7e5a81c308243ef0bef8faeedf8d683296edac86823f93acbcb7c1` |
| `docs-viewer-recording.html` | `0793762ac2c36162193d5053de5b67c4387423e61b93c6556401a3d0f0e2b679` |
| `docs-viewer (1).html` | `b3afe55ffc37e9447e91e57d3317bcd1a7425467a52c94cdf0065835580907ed` |
| `NES_EDU_Markdown_Viewer_Final.html` | `19e68e534c45cbaf04ddd2a982039312bdeaa4b3bb9222960c9e4f4fad1026ba` |
| `NES_EDU_Markdown_Viewer_Visual_Edit_Final.html` | `9d74e486b788f4d5e4d745b58e0778654edb853e435174f519759c41b61cefa4` |
| `NES_EDU_Markdown_Viewer_Complete_Final.html` | `5e85f19235bede6d4eaad369fa908d29d9fd0f522ddf2fdee5d3dd24f0231f3a` |

## أساس التحقق وحدوده

المصادر الستة من exports المستعادة تطابق بصمات خطة الإصدارات وبايتات محتوى استجابات الوسوم المحفوظة. طوبق مسار كل رابط محفوظ مع الوسم واسم الملف. هذا تحقق محلي من الأدلة المسجلة؛ لم يحدث اتصال GitHub جديد أو تشغيل للمصادر أثناء إعداد هذه الوثائق. فحص الصياغة السابق لا يثبت سلوك وقت التشغيل أو سلامة التصدير. لم تتغير المصادر الأصلية، ولم تُصلح هذه الوثائق عيوبها.

