# Behavioral Interoperability Testing Ontology (BITO)

**Version:** 1.0.0  
**Status:** Review version  
**Namespace:** `https://w3id.org/bito#`  
**License:** CC BY 4.0


## Overview

The Behavioral Interoperability Testing Ontology (BITO) provides a lightweight semantic model for ontology-driven behavioral interoperability testing. It represents the links between expected scenario behavior, observed execution evidence, behavioral constraints, validation results, and verdicts.

BITO is designed as a reusable behavioral interoperability testing layer that can complement domain ontologies and support the validation of runtime behavior against expected scenario rules.


## Repository contents

This folder contains the ontology-level artifacts for BITO, including the ontology files, documentation, diagrams, competency questions, SPARQL/DL queries, and ontology validation evidence.

```text
Behavioral Interoperability Testing Ontology (BITO)/
│
├── README.md
├── ontology/
├── documentation/
├── conceptual-diagram/
├── competency-questions/
├── sparql-dl-queries/
└── ontology-validation/
```

## Folder description

| Folder                  | Description                                                                                                                                                      |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `ontology/`             | Contains the BITO ontology files, including the main ontology serialization files.                                                                               |
| `documentation/`        | Contains generated ontology documentation, including WIDOCO-based documentation when available.                                                                  |
| `conceptual-diagram/`   | Contains conceptual diagrams representing the main BITO classes, relations, and modeling structure.                                                              |
| `competency-questions/` | Contains the competency questions used to define and assess the intended scope of the ontology.                                                                  |
| `sparql-dl-queries/`    | Contains SPARQL and DL queries used to check whether the ontology and its example data can answer the competency questions.                                      |
| `ontology-validation/`  | Contains ontology validation and verification evidence, including OOPS! pitfall checking, HermiT consistency checking, and competency-question checking results. |


## Funding acknowledgement

This work is prepared in the context of the HEDGE-IoT project, funded by the European Union's Horizon Europe research and innovation programme under Grant Agreement No. 101136216.
