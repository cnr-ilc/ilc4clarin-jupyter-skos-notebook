# REALITER Notebooks

This folder contains a collection of Jupyter Notebooks developed to support the conversion and publication of terminological data from the **REALITER** network into SKOS (Simple Knowledge Organization System) RDF format.

The notebooks are intended as practical, modular tools to assist in transforming tabular representations of multilingual terminological resources—produced within the REALITER context—into structured and interoperable Linked Open Data.

## About REALITER

[REALITER](http://www.realiter.net) is the Pan-Latin Terminology Network, which brings together individuals, institutions, and organizations from Romance-language-speaking countries who work in the field of terminology.

The network's **main objective** is to foster the harmonious development of Romance languages, based on their common origin and shared lexical formation mechanisms.

More specifically, REALITER seeks to:
- Establish shared methodological principles for the co-creation of terminological products.
- Conduct joint research and develop tools to support Romance language development.
- Produce multilingual terminological resources in socially relevant fields.
- Share reference documentation and materials.
- Promote reciprocal training through exchanges of experts, trainers, students, and educational resources.

REALITER is structured into an Assembly, a Committee, a Secretariat, and working groups responsible for coordinating joint projects. The Secretariat is currently hosted at the Università Cattolica del Sacro Cuore in Milan, under the direction of Prof. Maria Teresa Zanola.

One of the network's central missions is to advocate for the continued development and visibility of scientific and technical terminologies in Romance languages, as a counterbalance to the increasing dominance of English in scholarly communication.

## Notebooks Overview

The notebooks included in this folder are focused on the following tasks:

- **Parsing and cleaning** multilingual tabular datasets (e.g., CSV, Excel).
- **Modeling terminologies** using SKOS concepts and relationships.
- **Generating multilingual labels, definitions, and notes** in accordance with SKOS best practices.
- **Exporting RDF data** in Turtle serialization, ready for publication in LOD platforms.

Each notebook is designed to be modular, extensible, and adaptable to different terminological domains and multilingual configurations.

## Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Dependencies (install via `pip install -r requirements.txt`):
  - `rdflib`
  - `pandas`
  - `openpyxl` (for Excel support)
  - `tabulate` (optional, for pretty-printing tables)

## How to Use

1. Place your tabular terminology data (in CSV or XLSX format) into the input folder.
2. Open and run the notebooks step by step.
3. Configure the concept scheme and multilingual properties as needed.
4. Export the RDF output for use in triple stores, vocabulary browsers, or data portals.

Each notebook includes inline documentation and examples.

## License

[![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## References

- **Zanola, M., Calvi, S., Dankova, K., & Marzo, L.** (2023).  
  *Risorse terminologiche plurilingui nel rispetto dei principi FAIR del web semantico*.  
  In *Working Papers*, pp. 90–92. ISBN: 9788875902681.  
  This work describes the transformation of REALITER multilingual terminological resources into FAIR-compliant formats, in collaboration with CLARIN-IT.  

---
