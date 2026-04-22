# SIGGRAPH Asia 2026 Writing Project

This repository is a clean LaTeX writing scaffold for an ACM SIGGRAPH Asia 2026 technical paper submission.

## Current template choice

This scaffold follows the current ACM/SIGGRAPH technical-paper review format:

- ACM double-column layout
- `acmart` class with `acmtog` style
- anonymous review mode
- explicit submission ID placeholder

Current root file:

- `main.tex`

## Important author-instruction assumptions

The setup is aligned to the current SIGGRAPH technical-paper author instructions and template guidance:

- use `\documentclass[acmtog,anonymous,review]{acmart}`
- add `\acmSubmissionID{...}` after a paper ID is assigned
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
- Generated PDFs are gitignored by default. Remove that rule later if you decide to version the compiled submission.
