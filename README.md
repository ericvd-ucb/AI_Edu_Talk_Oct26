# AI_Edu_Talk_Oct26

Slide deck for **"Teaching AI the Way We Teach Data Science: Open, hands-on, built to scale"**, Eric Van Dusen (UC Berkeley CDSS), AI at Sciencepark, LAB42 Amsterdam, October 9, 2026.

**VibeSlides:** this talk was built in conversation with both ChatGPT and Claude, and built in Quarto with Claude Code. I was trying to learn an open-tools approach to slides, to move off of G&&gle Slides and to teach myself a Markdown-based workflow (as I have learned, Markdown is the language the models think in). It was not simple or easy, nor does it feel done yet, but hopefully it is a long-term play that I can build on over time.

## Slides

**View online:** https://ericvd-ucb.github.io/AI_Edu_Talk_Oct26/ (opens the combined deck)

Press `S` for speaker notes, `F` for fullscreen. Each HTML file is self-contained: download and open it in a browser, no internet needed.

### Combined deck (the talk)

The best of both drafts below, 17 slides in three parts: what we know works, can we adapt what we teach, and what investments we need.

- **HTML:** [`amsterdam-combined.html`](amsterdam-combined.html)
- **PDF:** [`amsterdam-combined.pdf`](amsterdam-combined.pdf)
- **Source:** [`amsterdam-combined.qmd`](amsterdam-combined.qmd)

### Earlier draft A: "Teaching AI the Way We Teach Data Science"

Demo-focused version: small models in code, on a JupyterHub, and in the browser.

- **HTML:** [`amsterdam.html`](amsterdam.html) · online: https://ericvd-ucb.github.io/AI_Edu_Talk_Oct26/amsterdam.html
- **PDF:** [`amsterdam.pdf`](amsterdam.pdf)
- **Source:** [`amsterdam.qmd`](amsterdam.qmd)

### Earlier draft B: "AI Education at Scale"

Argument-focused version: from algorithms to systems, and who owns the laboratory.

- **HTML:** [`amsterdam-ai-university.html`](amsterdam-ai-university.html) · online: https://ericvd-ucb.github.io/AI_Edu_Talk_Oct26/amsterdam-ai-university.html
- **PDF:** [`amsterdam-ai-university.pdf`](amsterdam-ai-university.pdf)
- **Source:** [`amsterdam-ai-university.qmd`](amsterdam-ai-university.qmd) (styles in `slides.css`)

## Rebuilding

```bash
quarto render amsterdam-combined.qmd
quarto render amsterdam.qmd
quarto render amsterdam-ai-university.qmd
```

To regenerate the PDF (uses [DeckTape](https://github.com/astefanutti/decktape), needs Node):

```bash
npx decktape@3 reveal --size 1280x720 --load-pause 1500 "file://$PWD/amsterdam-combined.html" amsterdam-combined.pdf
```
