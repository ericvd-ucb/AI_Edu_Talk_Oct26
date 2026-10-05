# AI_Edu_Talk_Oct26

Slide deck for **"Teaching AI the Way We Teach Data Science: Open, hands-on, built to scale"**, Eric Van Dusen (UC Berkeley CDSS), AI at Sciencepark, LAB42 Amsterdam, October 9, 2026.

## Slides

**View online:** https://ericvd-ucb.github.io/AI_Edu_Talk_Oct26/

- **HTML (reveal.js):** [`amsterdam.html`](amsterdam.html). Download and open in a browser; it's self-contained. Press `S` for speaker notes, `F` for fullscreen.
- **PDF:** [`amsterdam.pdf`](amsterdam.pdf)
- **Source (Quarto):** [`amsterdam.qmd`](amsterdam.qmd)

## Rebuilding

```bash
quarto render amsterdam.qmd
```

To regenerate the PDF, open `amsterdam.html?print-pdf` in Chrome and print to PDF, or run headless Chrome:

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new \
  --no-pdf-header-footer --virtual-time-budget=15000 \
  --print-to-pdf=amsterdam.pdf "file://$PWD/amsterdam.html?print-pdf"
```
