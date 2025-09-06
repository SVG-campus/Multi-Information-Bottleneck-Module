# ORCID & Zenodo Integration Guide

This guide shows exactly how to connect your GitHub repository to Zenodo for DOI minting and keep your ORCID iD in sync.

## ORCID
- Your ORCID: https://orcid.org/0009-0004-9601-5617
- In ORCID, enable *Trusted parties* updates from Zenodo so new DOIs flow in automatically.

## Zenodo
1. Login and enable the specific GitHub repo under *GitHub*.
2. Ensure `.zenodo.json` and `CITATION.cff` are committed in the repo root.
3. Create a GitHub **release** (push a tag). Zenodo will archive the snapshot and mint a DOI.
4. Use the **concept DOI** badge in the README for a stable reference. Update badges with the real record id.

## Badges (replace with real record id)
```
[![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.{ZENODO_RECORD_ID}.svg)](https://doi.org/10.5281/zenodo.{ZENODO_RECORD_ID})
```
