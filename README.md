# ProblySUS Mini Project Report

This repository contains the LaTeX source for the **ProblySUS** mini project report. The report documents a multi-signal website security system for detecting scam, phishing, and fraudulent websites using threat intelligence, DNS analysis, content inspection, browser behavior analysis, and a browser extension.

## Contents

- `main.tex` is the master document that includes all chapters and front matter.
- Chapter files such as `chapter1_introduction.tex` and `chapter5_implementation.tex` hold the individual report sections.
- `title.tex`, `abstract.tex`, `declaration.tex`, `certificate.tex`, `Acknowledgement.tex`, and `references.tex` contain the front pages and supporting sections.
- The `images/` folder stores the figures used throughout the report.

## Build the PDF

If you have a LaTeX distribution installed, compile the report from the project root with:

```bash
latexmk -pdf main.tex
```

If `latexmk` is not available, you can use `pdflatex` manually:

```bash
pdflatex main.tex
pdflatex main.tex
```

Running the build more than once helps resolve references, table of contents entries, and figure numbering.

## Project Overview

ProblySUS is presented as a web-based security system with:

- A React frontend for URL submission and analysis results.
- A Flask backend for orchestration and scoring.
- Parallel analysis modules for fast and detailed risk assessment.
- A Chrome extension for scanning URLs during browsing.

## Notes

- Generated files such as `.aux`, `.toc`, `.lof`, and `.lot` are build outputs and do not need to be edited manually.
- The main report output is produced from `main.tex`.