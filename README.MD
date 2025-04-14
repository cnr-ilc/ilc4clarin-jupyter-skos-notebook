# ilc4clarin-jupyter-skos-notebook

This repository provides a collection of Jupyter Notebooks designed to support the conversion and creation of linguistic resources from tabular data formats (e.g., CSV, Excel) into [SKOS](https://www.w3.org/TR/skos-reference/) (Simple Knowledge Organization System) RDF representations.

## Purpose

The notebooks are developed in the context of the **ILC4CLARIN** infrastructure and aim to offer reusable and adaptable tools for researchers and institutions in the Digital Humanities and Linguistics communities. They are intended to facilitate the publication of controlled vocabularies and terminological resources as Linked Open Data (LOD).

## Key Features

- 📘 Step-by-step workflows for converting tabular data to SKOS.
- 🧠 Examples and templates for encoding linguistic concepts, hierarchies, and metadata.
- 🐍 Fully implemented in Python using standard libraries and RDF processing tools (e.g., `rdflib`, `pandas`).
- 💻 Ready to use within local or cloud-based Jupyter environments.

## Target Audience

This repository is especially useful for:
- Linguists and lexicographers working with structured vocabularies.
- Researchers in the Digital Humanities interested in LOD publication.
- Developers and data managers handling metadata conversion tasks.

## Notebooks Overview

Each notebook focuses on a specific task or use case, such as:
- **Basic SKOS conversion** from CSV.
- **Mapping hierarchical relations** (broader/narrower).
- **Enriching concepts** with multilingual labels, definitions, and notes.
- **Exporting RDF** in Turtle or other serializations.

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/ilc4clarin/ilc4clarin-jupyter-skos-notebook.git

## Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Recommended libraries:
  - `rdflib`
  - `pandas`
  - `openpyxl` (for Excel files)

Install dependencies with:
```bash
pip install -r requirements.txt
```

> A `requirements.txt` file will be included in the repository for convenience.

## Acknowledgments

These notebooks are part of the ongoing efforts within the **CLARIN-IT** and **ILC-CNR** initiatives to support the creation and dissemination of Linked Open Data for the Humanities.
