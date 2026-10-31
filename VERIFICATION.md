# Verification

Tested October 31, 2026 using installed Google Chrome in headless mode on macOS.

## Passed browser flows

- All three worksheet parts render.
- All embedded illustrations load.
- Pie number, keyboard, pointer, and unset values saved.
- Dynamic table row and column changes saved.
- Text autosave restores after reload.
- Trial table restores after reload.
- JSON download preserves complete state.
- JSON import restores answers and pies.
- Invalid JSON structure rejected without changing work.
- Compressed link validates within length cap.
- Submission link round trip includes text and pie values.
- Submission tables are read only.
- Submission viewer leaves saved browser progress untouched.
- Editing invalidates previous generated link.
- Print copy includes full long answer.
- Print copy includes full equation entry.
- Oversized generated links blocked with no copyable URL.
- Malformed incoming link fails visibly without falling back to local answers.
- Oversized incoming link blocked.
- Stale tab cannot overwrite another tab’s saved work.
- Storage failure is visible and worksheet remains editable.
- Backup remains available when browser storage fails.
- Corrupt stored progress is not silently overwritten.
- Mobile viewport has no page-wide horizontal overflow.
- No browser JavaScript errors.

- Pointer dragging and zero/full/unset/clamped pie values passed.
- HTML-like answer text remained inert.
- Local-file worksheet and embedded images worked; link generation correctly required hosting.

## Additional checks

- Compared the source documents: original worksheet text remains in the original order. Only the operational save/submit note was replaced; the scientific clarification was added adjacent to the unchanged carbon-10 prompt.
- All seven original embedded image occurrences retain identical source data.
- No CFL branding in index.html.
- Compressed payload expanding beyond 1 MB was blocked.
- Generated a real browser PDF with a 180-line answer. Extracted PDF text includes the final answer line, full equation product, student identity, trial-table response, and all three worksheet parts.
- First PDF page includes the title, identity, and Part I. Print layout was exercised with dark-mode preference too.
- Blank worksheet print output was nine pages in this Chrome environment. Page counts vary by paper size, browser, and answer lengths.

## Limits

No GitHub deployment, repository write, or live Canvas submission was performed. Canvas URL acceptance and PDF upload must be checked in the instructor's actual assignment. PhET links were preserved; interactive behavior of the externally hosted simulations was not tested. Browser checks were performed in Chrome, not Safari/Firefox or on physical mobile devices. The 390-pixel mobile layout was inspected in an emulated viewport. Browser storage is local and can be cleared; JSON backups remain necessary.
