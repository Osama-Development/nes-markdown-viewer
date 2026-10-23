# Preserved defects and limits

- Markdown rendering assigns Marked output to innerHTML without a sanitizer.
  Raw HTML and dynamic DOM interpolation make untrusted input unsafe. Use trusted
  documents; restored source deliberately does not fix this historical behavior.
- State 3 export walks rendered DOM text and loses Markdown detail: formatting,
  link targets, tables/code and list distinctions can be omitted or flattened.
  Editing the DOM is not an exact-source save and can be lost on rerender.
- Later source-span/visual mapping is heuristic, not a complete round-trip parser.
  Complex nested Markdown, repeated text and transformed Arabic cue markup need
  manual comparison after edits. Exact source bytes of the HTML do not establish
  exactness of future edited Markdown exports.
- Drafts are plaintext localStorage, may exceed quota or be unavailable, and are
  bound to browser origin. Filename-based identity can collide for same-name files;
  the draft fingerprint is noncryptographic. Export downloads do not overwrite the
  original disk file. Clearing site data can remove drafts.
- FileReader and fetch are asynchronous; rapid selections can race. file:// fetch
  restrictions and missing registry Markdown are expected reasons to use a picker.
- Reading time and word counts are estimates; empty text and Arabic tokenization
  are not rigorously measured. No accessibility/browser compatibility claim is made.
- CDN versions are unpinned in earlier states. Fonts/icons remain remote in later
  states, so complete offline presentation and dependency reproducibility are limited.
