<div align="center">

# ProfiLLM — Project Page

Source for the project website of
**ProfiLLM: Utility-Aligned Agentic User Profiling for Industrial Ride-Hailing Dispatch**

_Under submission to **VLDB**, Scalable Data Science track &nbsp;·&nbsp; Deployed on DiDi's production dispatcher_

</div>

<p align="center">
  <a href="https://profillm.github.io"><img src="https://img.shields.io/badge/Live_Page-profillm.github.io-1f6feb?style=flat-square&logo=githubpages&logoColor=white" alt="Live Page"></a>
  <a href="https://profillm.github.io/appendix.html"><img src="https://img.shields.io/badge/HTML_Appendix-A–Q-6e7781?style=flat-square&logo=readthedocs&logoColor=white" alt="HTML Appendix"></a>
  <a href="https://profillm.github.io/files/ProfiLLM_paper.pdf"><img src="https://img.shields.io/badge/Paper-PDF-8957e5?style=flat-square&logo=adobeacrobatreader&logoColor=white" alt="Paper PDF"></a>
  <a href="https://profillm.github.io/files/ProfiLLM_appendix.pdf"><img src="https://img.shields.io/badge/Appendix-PDF-2da44e?style=flat-square&logo=adobeacrobatreader&logoColor=white" alt="Appendix PDF"></a>
</p>

This repository hosts the static project page for ProfiLLM. It needs no build step: GitHub Pages serves the files verbatim. The live site is at **https://profillm.github.io**.

## What's here

| File / folder | Purpose |
|---|---|
| `index.html` | Landing page: abstract, highlights, method, result tables, claim→evidence map, BibTeX, and code links. |
| `appendix.html` | The full appendix (Sections A–Q), rendered in HTML with KaTeX, a sidebar table of contents, and linkable anchors. |
| `files/ProfiLLM_paper.pdf` | Extended paper (full version, with appendix). |
| `files/ProfiLLM_appendix.pdf` | Appendix-only PDF (compressed). |
| `static/images/*.png` | Figures, converted from the paper PDFs. |
| `static/pdfs/figs/*.pdf` | Vector versions of every figure, linked from the captions. |
| `.nojekyll` | Tells GitHub Pages to serve `static/` verbatim. |

## Code & data

The code and data are under enterprise review at DiDi and will be released, upon approval, in the [ProfiLLM code repository](https://github.com/ProfiLLM/ProfiLLM). Per DiDi's data-governance policy, raw ride-hailing data and proprietary system details cannot be shared; the release will cover the method and interfaces with anonymized feature names.

