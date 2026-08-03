# OsdagBridge — FOSSEE Internship Report

FOSSEE semester-long internship report by **Om Pathania**, documenting the work done on the
[**OsdagBridge**](https://github.com/Aditya-Donde/OsdagBridge) project — the bridge-design
extension of the Osdag steel-design software.

The report is written in LaTeX, one source file per chapter, and compiles into a single
**`report/main.pdf`**.

## Repository layout

```
OSDAG_SUMMER_REPORT/
├── report/            # the report (LaTeX source)
│   ├── main.tex       # preamble, title page, includes every chapter
│   ├── chapters/      # one .tex file per chapter + acknowledgments
│   ├── images/        # screenshots (see "Images" below)
│   └── README.md      # build details + list of images needed
├── Media/             # title-page logos (IIT Bombay, FOSSEE)
├── Reference/         # style reference only (not part of the report)
└── .gitignore
```

## What the report covers

The work is organised by feature area, in the order it was carried out:

1. Introduction (NMEICT, FOSSEE, Osdag, OsdagBridge)
2. OsdagBridge Overview & Setup
3. 3D CAD Viewer: Nodes & Grillage
4. Toolbar System & Navigation
5. Bridge Geometry & Shear-Stud Solver
6. Coordinate Axis in the 3D View
7. Design Report Generation
8. Report Plot Capture & Zoom
9. UI/UX Enhancements
10. Material Input Validators
11. Conclusion & Lessons Learned

Each chapter documents the relevant contribution with real code from the pull requests it was
built in.

## Building the PDF

Requires a LaTeX distribution (e.g. MacTeX / TeX Live).

```bash
cd report
latexmk -pdf main.tex        # recommended
# or:
pdflatex main.tex && pdflatex main.tex
```

Output: `report/main.pdf`. Clean build artifacts with `latexmk -c`.

## Images

Screenshots go in `report/images/` using the exact filenames referenced in the chapters (each
has a `%% IMAGE NEEDED:` comment next to it). Until a file is added, that figure renders as a
labelled placeholder box, so the report always compiles. The title-page logos already live in
`Media/`.
