# SIGGRAPH Asia 2026 Writing Project

This repository is a clean LaTeX writing scaffold for an ACM SIGGRAPH Asia 2026 technical paper submission.

## Current template choice

This scaffold follows the current ACM/SIGGRAPH technical-paper review format:

- ACM double-column layout
- `acmart` class with `acmtog` style
- anonymous review mode
- assigned submission ID: `papers_1817s1`

Current root file:

- `main.tex`

## Important author-instruction assumptions

The setup is aligned to the current SIGGRAPH technical-paper author instructions and template guidance:

- use `\documentclass[acmtog,anonymous,review]{acmart}`
- keep `\acmSubmissionID{papers\_1817s1}` in both `main.tex` and `supplement.tex` so the PDF displays the assigned ID `papers_1817s1`
- keep the review version anonymous
- prefer ACM/TAPS-accepted LaTeX packages only

Before submission, re-check the final SIGGRAPH Asia 2026 call and page-limit wording in case the Asia program publishes track-specific constraints that differ from the current SIGGRAPH guidance.

## Local build

### Command line

```powershell
cd E:\paper\SIGS\SIGGRAPHASIA26
latexmk -pdf main.tex
```

Output goes to:

- `build/main.pdf`

### VS Code

Recommended extension:

- `James-Yu.latex-workshop`

Open the repository folder in VS Code, then run:

- `LaTeX Workshop: Build LaTeX project`

The workspace is already configured to:

- use `latexmk`
- place artifacts in `build/`
- view the PDF inside VS Code

## Suggested writing layout

- `sections/abstract.tex`
- `sections/intro.tex`
- `sections/related.tex`
- `sections/method.tex`
- `sections/experiments.tex`
- `sections/limitations.tex`
- `sections/conclusion.tex`
- `references.bib`

## Notes

- `acmart.cls` and `ACM-Reference-Format.bst` are vendored locally for a stable build.
- Compiled review PDFs are versioned in `build/main.pdf` and `build/supplement.pdf` for review handoff; auxiliary build files remain ignored.
