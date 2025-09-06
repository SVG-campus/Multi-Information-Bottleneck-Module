# Multi Information Bottleneck Module (UPDATE)

**ORCID+Zenodo integration assets** for the *Multi‑Information Bottleneck (MIB) Module* repo.

> ORCID: [0009-0004-9601-5617](https://orcid.org/0009-0004-9601-5617) · Zenodo: connected to GitHub & ORCID

---

## Overview
We present a rigorous formulation and validation of a Multi-Information Bottleneck (Multi-IB) module designed to compress multiple predictive signals for robust portfolio decision-making. We detail the mathemat- ical theory, derive and describe the final form of the algorithm, im- plement large-scale empirical tests, and provide proofs of robustness

If you are looking for the paper, it is included in this repository (see `paper/` or the main PDF). 
Test pages/materials are available in the project and were used to validate the workflow.

### Why this folder exists
This `/` bundle adds everything you need so GitHub ⟷ Zenodo ⟷ ORCID play nicely:
- Machine‑readable metadata (`.zenodo.json`, `CITATION.cff`)
- Badges & how‑to‑cite
- Release checklist for DOI minting via Zenodo
- Contributor, conduct, and licensing docs

## Quick start (repo maintainer)
1. **Connect GitHub → Zenodo** (one‑time): in Zenodo, enable this GitHub repository.  
2. **Create a tagged release** on GitHub (e.g., `v1.0.0`). Zenodo will auto‑mint a DOI.
3. **Add the DOI badge**: replace `{ZENODO_RECORD_ID}` in badges once the DOI exists.
4. **ORCID auto‑import**: in ORCID, add the new DOI; or enable auto‑update from trusted parties (Zenodo).

### Installation (optional for code users)
```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
# then use the module as documented below
```

## Minimal usage sketch (illustrative)
```python
# from mib_module import MultiInformationBottleneck

# mib = MultiInformationBottleneck(beta=1.0, views=2, estimator="variational")
# z = mib.encode(x_view1, x_view2)         # representation
# loss = mib.objective(z, y)               # bottleneck objective
# loss.backward()
```

> Replace with your repo's actual module paths once merged.

## Tests / Example pages
The project contains test material in:
- `.`

Use them to validate preprocessing and reproduction of key figures.

## Citation
After the Zenodo DOI is minted, cite as:

```
@software{{CITATION_KEY}},
  author    = {Santiago de Jesus Villalobos-Gonzalez},
  title     = {{REPO_TITLE}},
  year      = {{YEAR}},
  publisher = {Zenodo},
  version   = {{VERSION}},
  doi       = {{DOI}},
  url       = {{RELEASE_URL}}
}
```

A human‑readable `CITATION.cff` is included for GitHub’s citation UI.

## Badges
[![ORCID](https://img.shields.io/badge/ORCID-0009--0004--9601--5617-brightgreen)](https://orcid.org/0009-0004-9601-5617)
[![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.{ZENODO_RECORD_ID}.svg)](https://doi.org/10.5281/zenodo.{ZENODO_RECORD_ID})

## Licensing
- **Code:** MIT License (`LICENSE`).
- **Paper, figures & text:** CC BY 4.0 (`LICENSE-PAPER`).
Edit if you prefer a different scheme.

## Repo housekeeping
- `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md` set the tone for PRs and issues.
- `CHANGELOG.md` follows Keep‑a‑Changelog.
- `RELEASE_CHECKLIST.md` documents the exact Zenodo/ORCID release steps.

---

### Maintainer
**Santiago de Jesus Villalobos-Gonzalez** · ORCID [0009‑0004‑9601‑5617](https://orcid.org/0009-0004-9601-5617)

*This folder was auto‑generated to be dropped into the repository root.*
