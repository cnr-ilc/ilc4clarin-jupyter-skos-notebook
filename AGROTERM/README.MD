# AGROTERM Notebooks

This folder contains a collection of Jupyter Notebooks developed to support the transformation, enrichment, and publication of the **AGROTERM** resource as SKOS (Simple Knowledge Organization System) Linked Open Data (LOD).

The notebooks offer a practical, step-by-step workflow for converting a structured Excel-based terminology from the **MADIN TERM** project into RDF, adhering to semantic web standards and FAIR data principles.

## About AGROTERM

**AGROTERM** is a multilingual agricultural terminology developed within the framework of the MADIN TERM initiative, which focuses on the curation, standardization, and dissemination of terminological resources in socially and culturally relevant domains.

This particular resource emphasizes regional, certified, and domain-specific agri-food terms, with multilingual definitions and rich metadata. It is designed to be interoperable and reusable by leveraging SKOS and related semantic technologies.

AGROTERM includes:
- Terminological entries (concepts) in Italian, Spanish, and English.
- Definitions, morphological notes, and source references.
- Regional and domain-specific classifications (e.g., regions, certifications, domains).
- Metadata conforming to DC and DCT standards.

The vocabulary is published at:  
[https://vocabs.ilc4clarin.ilc.cnr.it/vocabularies/madin-term/agroterm/](https://vocabs.ilc4clarin.ilc.cnr.it/vocabularies/madin-term/agroterm/)

## Notebooks Overview

The Jupyter Notebooks provided in this folder carry out the following tasks:

- **Loading and cleaning** metadata and concept data from Excel sheets.
- **Structuring JSON resources** from tabular input.
- **Constructing YARRRML mappings** to represent concepts, labels, notes, collections, and broader/narrower hierarchies.
- **Translating YARRRML to RML** using the `yatter` library.
- **Generating RDF (TTL format)** using `morph-kgc`.
- **Post-processing and validation** of RDF graphs (e.g., cleaning labels, asserting `skos:hasTopConcept`).
- **Quality assurance** to check collection consistency and member existence.

Each step is modular and fully commented for reuse in similar terminology-to-RDF conversion workflows.

## Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Dependencies (install with `pip install -r requirements.txt`):
  - `rdflib`
  - `pandas`
  - `openpyxl`
  - `ruamel.yaml`
  - `yatter`
  - `morph-kgc`

## How to Use

1. Place the input Excel file (`agroterm_2025_rev.xlsx`) in the `src/` folder.
2. Run the notebooks in order to:
   - Normalize and export the metadata and concepts into JSON.
   - Generate YARRRML mappings for SKOS concepts and collections.
   - Convert YARRRML into RML.
   - Materialize RDF triples using `morph-kgc`.
3. Use the RDF Turtle files for integration into triple stores, vocabulary browsers (e.g., Skosmos), or semantic APIs.

All notebooks include comments and outputs to guide interpretation and adaptation.

## License

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## References

- **MADIN TERM**: A project promoting the development and sharing of cultural, scientific, and social terminologies in Italy.
- **SKOS (W3C Recommendation)**: [https://www.w3.org/TR/skos-reference/](https://www.w3.org/TR/skos-reference/)
- **morph-KGC**: A Python engine for materializing RDF from RML and YARRRML mappings — [https://github.com/oeg-upm/morph-kgc](https://github.com/oeg-upm/morph-kgc)