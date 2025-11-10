# Sleep Manuscript

This repository collects the LaTeX sources for the *Sleep* manuscript. The parts are organized so that each part's framing lives in its own wrapper file (`part1/part1.tex`, `part2/part2.tex`, `part3/part3.tex`).

## Branches

The branch `feature/modularized-parts` contains the modularized structure for Parts I–III. To review it locally, fetch the branch and check it out:

```bash
git fetch origin feature/modularized-parts
git checkout feature/modularized-parts
```

## Building the PDF

The project expects a standard LaTeX toolchain (for example, `latexmk` with `pdflatex`). Run the following from the repository root:

```bash
latexmk -pdf main.tex
```

If `latexmk` is unavailable, you can fall back to invoking `pdflatex` manually until references settle.

The generated `main.pdf` will appear alongside `main.tex` in the repository root.
