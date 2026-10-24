# NES EDU Markdown Viewer — preserved snapshot 6/6

Adds structure selection and source-range operations for cards, headings, line/paragraph breaks and separators, plus named Markdown download.

Open `NES_EDU_Markdown_Viewer_Complete_Final.html` in a modern browser and choose a local `.md`, `.markdown` or `.txt`
file. For registry-based fetching, serve this directory with
`python3 -m http.server 8000` and open the HTML at `http://localhost:8000/`
(URL-encode spaces). The registry's Markdown documents are not part of these
six recovered HTML files; use the file picker or provide your own documents.
There is no build, package installation, backend or deployment requirement.
External Google Fonts and Font Awesome assets require network access; states
1–3 also require the unpinned Marked CDN script. Later parser bundles are local.

Only the selected stage HTML is present in this commit; earlier originals remain in earlier commits. The original filenames and HTML bytes are preserved. `SHA256SUMS` identifies the selected file; `SNAPSHOTS.json` records chronology through this stage and identifies recovered sources and their observed creation
timestamps. Those timestamps order the recovered artifacts; they do not prove
developer commit dates, release dates or authorship. Git commits are new,
present-day restoration records by Restoration Bot, not reconstructed original
developer commits. Removing the preceding filename and adding the selected filename is a restoration path transition, not evidence of an original Git rename. Owner-authenticated remote Work commits are separate transport
records and can have different authors, timestamps and SHAs from local preparation.

See `ARCHITECTURE.md`, `FUNCTIONS.md`, `LIMITATIONS.md`, and `VERIFICATION.md`.
`MARKED-LICENSE.txt` covers Marked only; no application license was inferred.


## دليل الزائر والأدلة

- [التشغيل والاستخدام والحفظ والتصدير](RUNBOOK.md)
- [تاريخ اللقطات والإصدارات](ARCHIVE_HISTORY.md)
- [فهرس الدوال بنطاقات الأسطر](FUNCTION_LINE_INDEX.json)
- [فهرس الفروق السطرية الخمسة](LINE_DIFF_INDEX.json)

هذه إضافات توثيق حالية؛ تظل Tags التاريخية ثابتة مع وثائق حالتها الأصلية. لم تُجر اختبارات تشغيل؛ راجع القيود قبل استخدام Markdown غير موثوق.
