# Grounded LLM-Assisted NDR and EDR Alert Correlation

This repository contains the experimental notebook and supporting material for a master's thesis on improving Security Operations Centre triage using machine learning based detection, deterministic NDR and EDR alert correlation, and grounded LLM-assisted contextual analysis.

## Thesis Topic

**Enhancing Network and Endpoint Detection and Response Systems: A Grounded LLM-Assisted Contextual Analysis**

The project explores how fragmented NDR and EDR alerts can be correlated into structured incidents and enriched with evidence-based LLM narratives for faster SOC triage.

## Project Overview

Modern SOC teams often receive large volumes of isolated network and endpoint alerts. This project demonstrates a post-detection workflow that:

- Applies ML models to detect suspicious network behaviour.
- Correlates NDR and EDR alerts into structured incident bundles.
- Uses grounded LLM prompts to generate SOC-style summaries.
- Maps incident narratives to investigation context and recommended response steps.
- Compares cloud and local LLM behaviour for privacy and operational trade-offs.

## Key Components

- `notebooks/` - thesis experiment notebook.
- `docs/` - thesis PDF or public thesis link.
- `reports/` - generated SOC incident reports and result summaries.
- `data/` - dataset notes only. Do not upload large raw datasets or restricted logs.

## Methods Used

- Random Forest
- XGBoost
- Isolation Forest
- Autoencoder-style reconstruction
- NDR and EDR alert fusion
- MITRE ATT&CK aligned incident narrative generation
- Grounded LLM prompting

## Main Results

The experimental workflow showed that structured alert correlation can reduce fragmented telemetry into a smaller number of incident bundles. Grounded LLM analysis can then produce concise SOC-style narratives, missing-evidence lists, and recommended investigation steps while reducing analyst workload.

## Security Notice

Do not commit API keys, private datasets, personal credentials, cloud tokens, or sensitive logs. Use environment variables for API access.

Example:

```bash
export GEMINI_API_KEY="your_api_key_here"
```

In Python:

```python
import os

api_key = os.getenv("GEMINI_API_KEY")
```

## How to Run

1. Clone the repository.
2. Create a virtual environment.
3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Add required API keys as environment variables.
5. Open the notebook:

```bash
jupyter notebook notebooks/thesis_experiment.ipynb
```

## Repository Purpose

This repository is intended to show the research workflow, experiment logic, and security analysis approach used in the thesis. It is suitable for academic review, cybersecurity portfolio presentation, and future development of SOC automation concepts.

