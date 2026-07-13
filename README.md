# Operationalizing AI Risk Mitigation: A Taxonomy‑Driven Analysis of Open‑Source LLM Tools

This repository contains the code, data, and supplementary materials for the paper:

**Operationalizing AI Risk Mitigation: A Taxonomy‑Driven Analysis of Open‑Source LLM Evaluation and Security Tools**

*Afreen Alam, Evgenija Popchanovska, Ana Gjorgjevikj, Maryan Rizinski, Lubomir T. Chitkushev, Irena Vodenska, Dimitar Trajanov, 2026.*

The study proposes a taxonomy‑driven protocol for mapping open‑source LLM tooling to a comprehensive AI risk mitigation framework, with a particular focus on high‑stakes sectors such as financial services.

**This repository hosts the materials related to:**
- Prompts used to map the capabilities of 21 open‑source tools (e.g., Promptfoo, Garak, PyRIT, NeMo Guardrails, Langfuse, Arize Phoenix) to the 32 sub‑categories of the Extended MIT AI Risk Mitigation Taxonomy via NotebookLM.
- Conduct a human validation study (25% stratified sample, three reviewers) to determine the inter-rater agreeability of the automated mappings (accuracy, precision, recall, F1, Fleiss’ Kappa).

**Repository structure**
```text
.
├── data/
│   ├── tool_taxonomy_matrix.xlsx        # Tool×Risk capability matrix and human validation sample
│   ├── tool_metadata.csv               # Tool names, URLs, adoption metrics, inclusion/exclusion flags
│   ├── taxonomy_definitions.csv        # Extended MIT AI Risk Mitigation Taxonomy (32 subcategories)
│   ├── Manual Review of LLM Mappings.xlsx # Human validation of LLM taxonomy mappings of tool's capabilities to MIT taxonomy
│   └── Inter_rater_comparision.xlsx # Fleiss’ Kappa implementation preparation (input used in Fleiss_Kappa_Calculator.ipynb)
├── notebooks/
│   ├── Validation_selection.ipynb           # Script to generate validation subset
│   └── Fleiss_Kappa_Calculator.ipynb  # Fleiss’ Kappa implementation for 3 raters
├── prompts/
|   ├── anchor_prompt.txt                   # Single-Tool Anchor prompt used in NotebookLM
│   ├── extraction_prompt.txt               # Single-Tool Extract prompt used in NotebookLM
│   ├── synthesis_prompt.txt                # Matrix synthesis and taxonomy mapping instructions
│   └── summary_prompt.txt                  # Used to summarize tools' documentations for initial mapping validation
├── dashboard/
│   └── index.html                          # Published dashboard version of the analysis 
├── README.md
└── LICENSE
```
