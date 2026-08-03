# OsdagBridge Internship Report — Om Pathania

A LaTeX report documenting the work done on the **OsdagBridge** project during the
FOSSEE semester-long internship. The source is split one file per chapter under
`chapters/`; everything compiles into a single **`main.pdf`**.

## Layout

```
report/
  main.tex              # preamble, title page, \include of every chapter
  chapters/
    acknowledgments.tex
    00_intro.tex        # Ch1  Introduction
    01_setup.tex        # Ch2  OsdagBridge Overview & Setup
    02_cad_viewer.tex   # Ch3  3D CAD Viewer: Nodes & Grillage
    03_toolbar.tex      # Ch4  Toolbar System & Navigation
    04_geometry.tex     # Ch5  Bridge Geometry & Shear-Stud Solver
    05_axis.tex         # Ch6  Coordinate Axis in the 3D View
    06_report_gen.tex   # Ch7  Design Report Generation
    07_plot_capture.tex # Ch8  Report Plot Capture & Zoom
    08_ui_polish.tex    # Ch9  UI/UX Enhancements
    09_validators.tex   # Ch10 Material Input Validators
    10_conclusion.tex   # Ch11 Conclusion & Lessons Learned
  images/               # screenshots (see list below)
```

## Build

```bash
cd report
latexmk -pdf main.tex        # recommended
# or:
pdflatex main.tex && pdflatex main.tex
```

Output: `main.pdf`.

## Images still needed

Drop these into `images/` using the exact filename shown in each `\includegraphics`
(a `%% IMAGE NEEDED:` comment sits next to every placeholder in the chapters).
Until an image is added, compilation will warn about a missing file but still produce
the PDF with a blank box.
