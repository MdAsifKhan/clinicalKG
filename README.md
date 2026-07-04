# clinicalKG — GenEHR decoder knowledge graphs

Static interactive site of decoder-conditional association graphs from the GenEHR
EHR foundation model. Each `*.html` under the model directories is a fully
self-contained canvas app (graph data embedded inline). Served via GitHub Pages at
https://mdasifkhan.github.io/clinicalKG/

Contents:
- `r2_eval_min4/`, `r4_eval_v2_min4/`, `v1a_noFocal_eval_v1a_min4/` : five views each
  (conditional, cross-modal, cross-modal mass, mass topk, mass disparity).
- `index.html` : landing page.

Regenerated from the GenEHR repo with
`InteractiveKG/rerender_decoder_kg_site.py --hide-ai` (the Ask Claude panel is hidden
because a static host has no backend).
