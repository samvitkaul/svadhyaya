# Applying this update to the existing GitHub repository

**This folder is an additive patch, not a fresh repository.** Its structure is relative to the root of `samvitkaul/svadhyaya`. No existing file is overwritten by the patch.

1. Clone or open your existing local checkout:

   ```bash
   git clone https://github.com/samvitkaul/svadhyaya.git
   cd svadhyaya
   ```

2. Copy the `docs/`, `explorations/` and `questions/` folders from this update into the root, *merging directories* (not replacing them). Do **not** copy this instruction file unless you want it in the repo.
3. Inspect the additions, then push:

   ```bash
   git status
   git diff --check
   git add docs/ explorations/ questions/
   git commit -m "Add historical explorations and Obsidian visualization guide"
   git push origin main
   ```

The GitHub connection allowed reading the repo but returned HTTP 403 on file writes in this session. **Nothing in this update has been pushed automatically.**

Read [Obsidian visualization guide](docs/visualization-guide.md) and [historical ingestion policy](docs/historical-ingestion-policy.md) after copying.
