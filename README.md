# Resume

My resume, maintained in LaTeX and automatically compiled to PDF using GitHub Actions.

## Files

- `resume.tex` — Source file for the resume.
- `pdf/resume.pdf` — Generated resume PDF.
- `.github/workflows/build.yml` — Workflow that compiles the PDF whenever `resume.tex` changes on `main`.

## Build locally

Install a LaTeX distribution, such as TeX Live, and run:

```bash
mkdir -p pdf

pdflatex -interaction=nonstopmode -halt-on-error \
  -output-directory=pdf resume.tex

pdflatex -interaction=nonstopmode -halt-on-error \
  -output-directory=pdf resume.tex