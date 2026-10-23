# Application function index

Extracted from preserved application code, starting at showToast; embedded Marked
internals are excluded. File/UI functions load files and navigate; preprocess and
render functions transform presentation; draft/state functions persist source;
editing functions map and patch text; structure functions operate on selected spans.

## NES_EDU_Markdown_Viewer_Complete_Final.html

- `showToast()`
- `initCollapsiblePanels()`
- `initKeyboardNavigation()`
- `initFilesUI()`
- `selectFileByIndex()`
- `handlePickedFiles()`
- `sourceFingerprint()`
- `draftKey()`
- `loadDocumentState()`
- `persistDocument()`
- `updateDraftStatus()`
- `commitSourceEdit()`
- `commitVisualEdit()`
- `currentDocument()`
- `flushDocumentSave()`
- `preprocessSlideMarkdown()`
- `classifyToneClass()`
- `renderFormattedDocument()`
- `tokenizeSourceSpans()`
- `nodeMatchesToken()`
- `encodeInsertedText()`
- `rawIndexForDisplayed()`
- `mapEditableLeaves()`
- `bindVisualEditor()`
- `enableInlineEditing()`
- `exportCurrentMarkdown()`
- `downloadMarkdownNamed()`
- `toggleStructurePanel()`
- `getSelectedSpan()`
- `currentSelectedKind()`
- `bindStructureSelection()`
- `selectStructureBlock()`
- `activateSelectedPosition()`
- `updateStructureUI()`
- `patchSourceRange()`
- `newCardSource()`
- `insertNewCard()`
- `deleteSelectedCard()`
- `changeCardMetadata()`
- `insertNewHeading()`
- `changeHeadingLevel()`
- `insertedAtLineEnd()`
- `insertStructuralLine()`
- `setupScrollSpy()`
- `highlightTOCItem()`
- `scrollToSection()`
- `filterTOC()`
- `navigateAdjacentFile()`
- `adjustFontSize()`
- `resetFontSize()`
