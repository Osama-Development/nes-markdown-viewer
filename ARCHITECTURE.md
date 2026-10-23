# Architecture

Each snapshot is a standalone HTML application with embedded CSS and JavaScript.
The shared flow is file registry/picker → FileReader or fetch → cached Markdown →
Arabic slide preprocessing → Marked HTML → DOM layout, TOC and navigation.
No server writes the chosen files. Downloads use browser Blob/object URLs.

States 1–2 are viewers. State 3 edits rendered elements and reconstructs export
text from DOM children. State 4 introduces a documentStates Map with original,
source and exported strings plus source-span mapping and source editors. States
5–6 map editable leaves to source spans, patch source text, then persist drafts;
state 6 adds structural source-range patches. Draft identity uses filename and a
fast noncryptographic fingerprint of original text. LocalStorage contains source
and exported strings in plaintext. This is local browser persistence, not a file
save or cloud backup. No framework or module bundler is present.
