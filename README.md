[README.md](https://github.com/user-attachments/files/34220814/README.md)
# nuclear-chemistry-simulations
Interactive nuclear chemistry simulation worksheets
# Nuclear Chemistry Simulations: CHMY 121 Interactive Worksheet

A self-contained, no-build, browser-only pilot of the eight-page nuclear simulation worksheets. It follows the original **Part I Alpha Decay**, **Part II Beta Decay**, and **Part III Radioactive Dating** sequence, preserving the written-response prompts, four adjustable pie charts for predictions and four for observations in each half-life investigation, and editable observation/trial tables.

## Publish using GitHub Pages
1. Create a new GitHub repository (e.g., `nuclear-chemistry-simulations`).
2. Upload `index.html` to the repository's root (or push the files with Git).
3. In the repository, open **Settings → Pages**, select **Deploy from a branch**, choose `main` and `/(root)`, then Save.
4. Open the GitHub Pages URL from Settings once deployed. No build tools or third-party JS libraries are needed.

## Student workflow
1. Open the web worksheet and enter name/section.
2. Open each linked PhET simulation and complete the questions.
3. Enter values into editable data tables and drag sliders to color pie charts.
4. Select **Save Backup** periodically to download a `.json` progress backup. **Restore Backup** reopens it later, including on a different computer.
5. Select **Print / Save PDF** and choose **Save as PDF** in the browser print dialog. Save the entire document, review the PDF for complete answers, and upload that single PDF to the existing Canvas assignment.

### Pilot notes and limitations
- **No submissions are sent automatically.** GitHub Pages is static hosting. Canvas remains the actual submission point.
- Student responses are saved only in the browser's `localStorage`. Clearing browser data, private browsing, switching devices, or device loss can erase that data. Downloaded JSON backups make recovery possible. The website does not transmit or store names or answers on GitHub.
- Browser printing is not guaranteed to behave identically across all browsers. Test in Chrome, Edge and Safari with long answers and all three parts before inviting students. The Print / Save PDF button invokes the browser's print dialog (it does not upload a file or synthesize PDFs on a server).
- Text input boxes support normal text and pasted Unicode isotope notation; there is not yet an equation editor or rich-text table insertion tool.
- The original worksheet repeated the label '2(a)' within Part II. This version uses 2(a)–2(f) for a unique sequence and fixes the accidentally repeated 'Part II' heading on radioactive dating to Part III.
- The original beta-decay section asks about **carbon-10**. Carbon-10 undergoes positron emission (β⁺), not the β⁻ process shown by the other examples. This version preserves the isotope and explains the distinction.
- The source's trial table says 'relative numbers of starting substance and decay product' without specifying table notation. This digital version asks for the count of **parent atoms remaining** per trial, with daughter atoms inferred as `40 - parent`.
- Pie charts are adjusted in whole percentages and the displayed atom counts are rounded estimates. Recorded values do not claim deterministic decay.
- This is a **volunteer pilot**, not a replacement for the original accessible downloadable PDF until tested by students.

## Files
- `index.html`: entire static application including CSS and JavaScript. No dependencies.
- `README.md`: setup and student/instructor guidance.

The original worksheet credits Trish Loeblein and Phil Cook, PhET Teaching Ideas and Activities (June 2020, AW). PhET simulations are linked externally and are not reproduced or hosted in this project.

## Compatibility with the first pilot
The existing browser storage key and JSON backup format intentionally retain their original internal identifiers so students can restore earlier work. These identifiers are not student-facing branding.
