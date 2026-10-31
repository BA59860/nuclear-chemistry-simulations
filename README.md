# Nuclear Chemistry Simulations

A buildless, unbranded CHMY 121 worksheet for GitHub Pages. All three parts, original question wording, embedded reference illustrations, editable pie charts, and dynamic tables from the supplied `nuclear-simulations.html` are retained. The earlier GitHub Pages prototype supplies the JSON progress-backup and recommended PDF-submission workflow.

## Appearance and navigation

Choose Light or Dark at the top. The initial appearance follows the device preference; the selected mode is remembered in this browser. Section buttons open Parts I, II, III or the complete worksheet. The last section is remembered too.

Autosave is enabled by default and saves on every answer change. “Save and continue” confirms browser saving before advancing. If saving fails or another tab conflicts, it keeps the section open with recovery guidance. Students can download a progress file for another device or as a backup. The final section offers “Save and finish worksheet,” then directs students to the PDF submission button. Printing includes every section regardless of the active screen section, and always uses a light print layout.

## Students: save and submit

1. Complete the worksheet while using the linked PhET simulations.
2. Check the save status at the bottom. Work is stored in this browser and site address, not in an account or on a server. Private browsing, browser cleanup, changing addresses, or changing devices can remove or isolate it.
3. Download **Save progress file** regularly. Use **Open progress file** to resume on another browser/device. Import asks before replacing current answers. JSON is a progress backup, not a PDF.
4. **Recommended:** choose **Print / Save PDF · Recommended**, select Save as PDF in the browser/system print dialog, review all three parts, and upload the PDF file to Canvas. Turn off browser headers/footers if desired. This is one PDF; students do not need to ZIP it. The downloadable ZIP in this package is for deploying the website.
5. Nothing is automatically sent to Canvas.

## Optional experimental submission links

Use only if the instructor accepts URL submissions. Generate a fresh link after editing, then copy it to Canvas. Links contain the student's name and entire worksheet, compressed but **not encrypted**. Anyone who receives a link can read it. History synchronization, clipboard tools, and the destination service may retain it. No shortener or server is involved.

- A complete URL is limited to **8,000 characters**, including its hosted base address. Longer links are blocked and cannot be copied. Incoming oversized links are also blocked. This is a conservative application policy, not a promise that Canvas or every browser accepts links of that length; PDF is preferred.
- Links require an HTTP(S) hosted page and a browser with native gzip `CompressionStream` / `DecompressionStream`. Unsupported browsers can still use the worksheet, backups, and PDF workflow.
- Links open a read-only snapshot. They never replace the viewer's locally saved worksheet. The viewer can print the snapshot or download its JSON backup. Opening a link does not prove that Canvas received it.
- The version-2 gzip link format is not compatible with the earlier Claude LZ-String `#s=` links. Unsupported, malformed, oversized, or invalid links show a visible error instead of displaying saved local answers.

## Deploy on GitHub Pages

Prepared for [BA59860/nuclear-chemistry-simulations](https://github.com/BA59860/nuclear-chemistry-simulations), serving [the worksheet site](https://ba59860.github.io/nuclear-chemistry-simulations/). Deployment is not verified until the updated files are committed and GitHub Pages finishes publishing.

1. Extract this ZIP. Place `index.html` at the root of the intended repository (or in its configured Pages folder). `README.md` and `VERIFICATION.md` may be included alongside it.
2. In the repository's **Settings → Pages**, select the intended branch and folder for deployment.
3. Visit the Pages address after deployment. Test a JSON download/import, PDF, and optional submission link on that exact address before assigning the worksheet.

There is no build command, npm dependency, API key, CDN script, analytics, or backend. Fonts use local fallbacks. Reference pictures are embedded in `index.html`. The worksheet runs from a downloaded file too; use the hosted address for consistent browser storage and to generate submission links. Internet access is needed to open PhET and reference sources.

## Recovery and validation

- Autosave writes immediately on edits. Storage errors stay visible; download a JSON backup if saving fails. A failed write leaves the visible answers available.
- Another tab changing the saved worksheet pauses autosave in the stale tab. Download that tab's JSON backup before using **Load saved browser copy**. This guards against ordinary conflicting edits; it is not a collaborative editor or transactional multi-user database.
- Unreadable or invalid stored data is left untouched. Restore a valid backup to recover; do not clear site data until recovery options are exhausted.
- JSON imports validate format, known answer fields, string values, table dimensions, fixed trial-table shape, and integer pie counts before replacing anything. File limit: 1,000,000 bytes. Dynamic tables support 1–100 rows and 1–12 columns. Worksheet answer data is limited to just under 1 MB; shorter responses improve usability.
- New backups use `format: "nuclear-chemistry-progress-v2"`, `savedAt`, and `answers`. Valid raw Claude autosave data under `chmy121-nuclear-sims-v1` is read on startup. The earlier `nuclearforge-pilot-v1` prototype has different fields and is **not** an import-compatible backup; keep those files separately. No speculative conversion is performed.
- Table-removal buttons ask before deleting the final row/column. Paste into editable cells inserts plain text. Imported and shared text is rendered as text, not HTML.
- Link decoding limits expanded data to 1 MB and validates the same schema as JSON import. Links are round-trip checked before being offered. Editing invalidates an already generated link.

## Scientific clarification

The original carbon-10 beta-decay prompt remains unchanged. A short adjacent note distinguishes positron emission (β⁺) from the β⁻ decay shown by the simulation. Source: [MIT OpenCourseWare, Radioactive Decay, Part II](https://ocw.mit.edu/courses/22-02-introduction-to-applied-nuclear-physics-spring-2012/0dedac3694d87c637b6214fd85c9eec9_MIT22_02S12_lec_ch7.pdf).

Original worksheet acknowledgment to Trish Loeblein and Phil Cook / PhET is retained. No CFL branding is present. No ownership or redistribution rights beyond the supplied materials are asserted.

See `VERIFICATION.md` for performed checks and their limits.
