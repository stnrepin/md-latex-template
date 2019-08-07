# Markdown+Latex with Pandoc

A template project which allows build PDF files from Markdown with Latex
snippets.

Now it works only on Unix-like platforms (Linux, Mac, etc.).

## Installation

1. Install make
2. Install pandoc
3. Install [Eisvogel](https://github.com/Wandmalfarbe/pandoc-latex-template)

Item 3 is optional, so you can work without it but then you have to edit
Makefile.

## Usage

Write your text into `doc.md` (you can also create multiple files, they will
be sorted and concatenated into single PDF), use `res` folder for resources
(images, others pdf, listings, etc.). Edit `titlepage.tex`. Use `style.yaml`
to configure appearance of PDF file.

Run make to build the project:

```bash
make
```

Result PDF-file is `out/doc.pdf`. You can change name of the output file in
Makefile (see TARGET variable).

Run `make clean` to clean up the workspace.
