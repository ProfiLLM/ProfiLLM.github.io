# ProfiLLM — Project Page

Static project page for **ProfiLLM: Utility-Aligned Agentic User Profiling for Industrial Ride-Hailing Dispatch** (VLDB 2027, Scalable Data Science track; deployed at DiDi Chuxing).

Live page: **https://profillm.github.io**

## Structure
```
index.html                    # landing page: abstract, highlights, method, result tables, claim→evidence map, BibTeX, code
appendix.html                 # FULL appendix (Sections A–Q), rendered in HTML with KaTeX; sidebar TOC, linkable anchors
.nojekyll                     # serve static/ verbatim on GitHub Pages
files/ProfiLLM_paper.pdf      # full paper (extended version, 20 pages, with appendix)
files/ProfiLLM_appendix.pdf   # appendix-only PDF (pages 11–20 of the extended version, compressed)
static/images/*.png           # figures (converted from the paper PDFs)
static/pdfs/figs/*.pdf        # vector versions of every figure (linked from captions)
```

Appendix section anchors (letters match the paper):
`#heterogeneity` A · `#case-studies` B · `#background` C · `#tools` D · `#algorithms` E ·
`#archetypes` F (`#cluster-viz` F.1) · `#simulator` G · `#wait-time` H · `#hourly` I ·
`#cluster-sensitivity` J · `#lambda` K · `#dpo-vs-exploration` L · `#offline-cost` M ·
`#complexity` N · `#extended-ab` O · `#privacy-fairness` P · `#prompts` Q

## Updating after a paper revision
1. Recompile `main.tex` (two passes), then refresh the PDFs:
   - `files/ProfiLLM_paper.pdf` ← compressed copy of `main.pdf`
   - `files/ProfiLLM_appendix.pdf` ← pages 11–20 of `main.pdf` (pdfseparate + pdfunite), compressed with Ghostscript `-dPDFSETTINGS=/printer`
2. If appendix text changed, update the corresponding section in `appendix.html` (content mirrors the tex verbatim; figure/table/equation numbers must match the compiled paper).

## Hosting (GitHub Pages, zero build)
This is a **user/organization site**: it resolves at `https://profillm.github.io` **only** if a GitHub
account/org named **`ProfiLLM`** owns a repo named **`ProfiLLM.github.io`** (GitHub lowercases the host).
1. Create a GitHub org/account named `ProfiLLM`.
2. Create a public repo `ProfiLLM.github.io` and push these files.
3. Settings → Pages → Build from `main` / root. Done.

If that name is unavailable, use a **project site**: push to a repo named `ProfiLLM` under any account →
served at `https://<account>.github.io/ProfiLLM` (then update the URL printed in the paper abstract).

## TODO before going live
- [ ] Push this directory to `ProfiLLM/ProfiLLM.github.io` and enable Pages (the paper's footnote URL currently 404s).
- [ ] Populate the **Code** repo (`github.com/ProfiLLM/ProfiLLM`) — it exists but is empty; the abstract promises code.
- [ ] After the submission PDF (8 pages + refs, appendix stripped) is frozen, decide whether the "Paper (PDF)" button
      should point to the submission version or keep the extended version.
