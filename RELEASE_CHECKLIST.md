# Release Checklist: GitHub ⟷ Zenodo ⟷ ORCID

## One-time setup
1. Log in to **Zenodo** and go to *GitHub* tab; **enable** this repository.
2. Ensure your **ORCID** iD is linked to Zenodo (Account → Linked accounts).

## For each release
1. Update `CHANGELOG.md` and bump version in your code (if applicable).
2. Commit the latest `CITATION.cff` and `.zenodo.json`.
3. Push a git tag, e.g.:
   ```bash
   git tag -a v1.0.0 -m "Initial release"
   git push origin v1.0.0
   ```
4. Wait for **Zenodo** to create a new **record** with a versioned DOI and a **concept DOI**.
5. Replace `{ZENODO_RECORD_ID}` in README badge with the actual record ID.
6. In **ORCID**, add works → *Add DOI* (or rely on Zenodo auto-update).

## Notes
- Zenodo reads `.zenodo.json` only on first upload for the **concept record**;
  subsequent releases inherit most metadata.
- Use the **concept DOI** to cite the project generally; the **version DOI** for a specific release.
