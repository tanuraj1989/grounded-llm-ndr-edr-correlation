# Thesis Summary

This thesis investigates how Network Detection and Response and Endpoint Detection and Response alerts can be correlated and contextualised to support faster SOC triage.

The workflow combines machine learning based detection, deterministic alert fusion, and grounded LLM-assisted analysis. Instead of using an LLM directly on isolated alerts, the system first groups related NDR and EDR events into structured incident bundles. The LLM then receives constrained evidence and produces short SOC-style narratives, missing-evidence notes, and recommended investigation steps.

The project focuses on the post-detection phase: reducing fragmented alerts, improving analyst context, and supporting more efficient investigation workflows.

