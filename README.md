# clinicalKG — genEHR cancer-onset graphs

Static site of decoder association graphs leading up to a first cancer diagnosis, from the genEHR
EHR foundation model. Served at https://mdasifkhan.github.io/clinicalKG/

Every sequence ends at the first cancer, so a cancer code never appears as a source and nothing
downstream of diagnosis can appear.

Contents:
- `index.html` — cohort selector (cancer / non-cancer / all patients).
- `graphs/<cohort>.html` — self-contained interactive graph, mass-corrected cPMI backbone.
- `figures/<cohort>_hub_page.*` — the learned-embedding map, then one row per cancer with a
  diagnosis neighbourhood and a cross-modal hub.
- `data/` — the tables behind the figures, including the per-cancer gate audit and the geometry
  noise-floor tests.

Built from the GenEHR repo with `genehrresults/gap_affinity_abc/build_site.py`, which reads the
three `affinity_graphs/gap_affinity_*_observed.npz` archives.
