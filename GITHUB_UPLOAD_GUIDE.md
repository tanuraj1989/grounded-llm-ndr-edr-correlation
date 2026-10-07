# GitHub Upload Guide

## Recommended Repository Name

`grounded-llm-ndr-edr-correlation`

## Short Description

Master's thesis experiment on NDR and EDR alert correlation using ML detection and grounded LLM-assisted SOC triage.

## Suggested Topics

`cybersecurity`, `ndr`, `edr`, `soc`, `machine-learning`, `llm`, `alert-correlation`, `mitre-attack`, `xgboost`, `random-forest`

## Before Uploading

1. Remove all hardcoded API keys from notebooks and scripts.
2. Revoke or rotate any key that was previously saved in a notebook.
3. Move raw datasets into a local-only `data/` folder.
4. Do not upload sensitive logs, private IP details, credentials, or cloud tokens.
5. Rename the notebook to something clean, for example:

```text
notebooks/thesis_experiment.ipynb
```

6. Add a short note explaining where public datasets can be downloaded.

## Suggested Structure

```text
grounded-llm-ndr-edr-correlation/
  README.md
  requirements.txt
  .gitignore
  .env.example
  notebooks/
    thesis_experiment.ipynb
  docs/
    thesis-summary.md
  reports/
    sample-soc-incident-report.md
```

## GitHub Web Upload Steps

1. Go to GitHub.
2. Click **New repository**.
3. Use the repository name above.
4. Add the short description.
5. Select **Public** if you want it visible for portfolio/recruitment.
6. Add `README.md`.
7. Upload sanitized notebook and supporting files.
8. Add repository topics from the list above.

## Git Command Line Steps

```bash
git init
git add README.md requirements.txt .gitignore .env.example GITHUB_UPLOAD_GUIDE.md
git commit -m "Initial thesis project repository"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/grounded-llm-ndr-edr-correlation.git
git push -u origin main
```

