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

## Appendix anchors

Section letters match the paper:

`#heterogeneity` A · `#case-studies` B · `#background` C · `#tools` D · `#algorithms` E ·
`#archetypes` F (`#cluster-viz` F.1) · `#simulator` G · `#wait-time` H · `#hourly` I ·
`#cluster-sensitivity` J · `#lambda` K · `#dpo-vs-exploration` L · `#offline-cost` M ·
`#complexity` N · `#extended-ab` O · `#privacy-fairness` P · `#prompts` Q

## Updating after a paper revision

1. Recompile `main.tex` (two passes), then refresh the PDFs:
   - `files/ProfiLLM_paper.pdf` ← compressed copy of `main.pdf`.
   - `files/ProfiLLM_appendix.pdf` ← appendix pages of `main.pdf` (`pdfseparate` + `pdfunite`), compressed with Ghostscript `-dPDFSETTINGS=/printer`.
2. If the appendix text changed, mirror it in the matching section of `appendix.html`. Figure, table, and equation numbers must stay in sync with the compiled paper.

## Hosting

This is a GitHub user/organization site: it resolves at `https://profillm.github.io` when an account or org named `ProfiLLM` owns a repo named `ProfiLLM.github.io` (GitHub lowercases the host). Push these files to that repo and enable **Settings → Pages → Deploy from `main` / root**.

If that name is unavailable, push to a repo named `ProfiLLM` under any account to serve a project site at `https://<account>.github.io/ProfiLLM`, and update the URL printed in the paper abstract accordingly.

## Related

- Code repository (release pending enterprise review): https://github.com/ProfiLLM/ProfiLLM
</content>
</invoke>
