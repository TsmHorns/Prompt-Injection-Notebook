# Prompt-Injection-Notebook

A Jupyter/Colab-based lab for testing, logging, and validating prompt injection attempts against large language models.
Supports **persistent chat** and one-shot **Scout** modes, schema-validated findings, auto-tagging of vulnerabilities, and visual analytics. Ideal for research, demonstration, and skill showcase in AI red teaming.

---

## **Features**

* **Chat Mode** – persistent conversation with memory.
* **Scout Mode** – one-shot prompts with no memory.
* **HF Router Client** – HuggingFace token support with automatic token rotation.
* **Schema Validation** – ensures JSON findings are consistent.
* **Auto-Tagging** – classifies prompt responses into vulnerability categories.
* **Findings Dashboard** – tables and charts for severity & model analysis.
* **Master Export** – aggregated JSON of all findings, with optional filter and de-duplication.
* **File Upload** – batch prompts from `.txt` files.

---

## **Requirements**

* Python 3.x (Jupyter or Colab)
* HuggingFace API token (supports multiple tokens, comma-separated)
* Optional packages: `ipywidgets`, `pandas`, `matplotlib`, `seaborn`, `plotly`, `altair`, `jsonschema`, `scikit-learn`

---

## **Quick Start**

1. Open the notebook in **Jupyter** or **Colab**.
2. Enter your HuggingFace token(s) in the **HF Token(s)** field.
3. Configure the **model**, **max tokens**, and **temperature**.
4. Type a prompt in **Chat** or **Scout** mode.
5. Click **☠️ Cast** (Chat) or **🎯 One-Shot** (Scout).
6. View logs, results table, and visual analytics.
7. Export findings via **📦 Export Master JSON**.
8. Download `master_findings.json` for offline analysis.

---

## **Notes**

* **Scout mode** is ideal for testing single-shot prompts.
* **Chat mode** keeps context for multi-step interactions.
* Auto-tagging provides a baseline classification of potential vulnerabilities.
* All findings are safely logged; no real prompt injections are included.

---
