# AI_Edu_Talk_Oct26

Slide deck for **"Teaching AI the Way We Teach Data Science: Open, hands-on, built to scale"**, Eric Van Dusen (UC Berkeley CDSS), AI at Sciencepark, LAB42 Amsterdam, October 9, 2026.

**Rig** This talk was built with Claude Code in VS Code - written in Quarto and deployed to gh-pages in an attempt to 1) move off of G%%gle Slides 2) learn to co-create slides with LLM 3) teach myself parts of open tool reproducible workflow with coding assistance.   It was not simple or easy or does it feel done, yet. But it hopefully is a long term play that I can build on over time.  

## Slides

**View online:** https://ericvd-ucb.github.io/AI_Edu_Talk_Oct26/

- **HTML (reveal.js):** [`amsterdam.html`](amsterdam.html). Download and open in a browser; it's self-contained. Press `S` for speaker notes, `F` for fullscreen.
- **PDF:** [`amsterdam.pdf`](amsterdam.pdf)
- **Source (Quarto):** [`amsterdam.qmd`](amsterdam.qmd)

## Second deck: "AI Education at Scale"

An alternate version of the talk ("What can we learn from data science?").

- **HTML:** [`amsterdam-ai-university.html`](amsterdam-ai-university.html) · view online: https://ericvd-ucb.github.io/AI_Edu_Talk_Oct26/amsterdam-ai-university.html
- **PDF:** [`amsterdam-ai-university.pdf`](amsterdam-ai-university.pdf)
- **Source:** [`amsterdam-ai-university.qmd`](amsterdam-ai-university.qmd) (styles in `slides.css`)

## Rebuilding

```bash
quarto render amsterdam.qmd
quarto render amsterdam-ai-university.qmd
```

To regenerate the PDF (uses [DeckTape](https://github.com/astefanutti/decktape), needs Node):

```bash
npx decktape@3 reveal --size 1280x720 --load-pause 1500 "file://$PWD/amsterdam.html" amsterdam.pdf
```
