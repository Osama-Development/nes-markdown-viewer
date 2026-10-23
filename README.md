# NES EDU Markdown Viewer — preserved snapshot 1/6

Arabic RTL Markdown viewer; file registry, file/folder picker, slide cues, table wrapping, heading TOC, font controls and adjacent-file navigation.

Open `docs-viewer.html` in a modern browser and choose a local `.md`, `.markdown` or `.txt`
file. For registry-based fetching, serve this directory with
`python3 -m http.server 8000` and open the HTML at `http://localhost:8000/`
(URL-encode spaces). The registry's Markdown documents are not part of these
six recovered HTML files; use the file picker or provide your own documents.
There is no build, package installation, backend or deployment requirement.
External Google Fonts and Font Awesome assets require network access; states
1–3 also require the unpinned Marked CDN script. Later parser bundles are local.

The original filenames and HTML bytes are preserved. `SHA256SUMS` and
`SNAPSHOTS.json` identify the materialized sources and their observed creation
timestamps. Those timestamps order the recovered artifacts; they do not prove
developer commit dates, release dates or authorship. Git commits are new,
present-day restoration records by Restoration Bot, not reconstructed original
developer commits. Owner-authenticated remote Work commits are separate transport
records and can have different authors, timestamps and SHAs from local preparation.

See `ARCHITECTURE.md`, `FUNCTIONS.md`, `LIMITATIONS.md`, and `VERIFICATION.md`.
`MARKED-LICENSE.txt` covers Marked only; no application license was inferred.
