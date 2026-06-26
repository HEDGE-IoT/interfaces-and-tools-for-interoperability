# Behavioral Interoperability Testing

This folder contains the artifacts for ontology-driven behavioral interoperability testing in the energy domain. The implemented example focuses on the Flexible Start use case, Scenario 3, where the expected behavior of a device is validated against observed evidence using RDF, RML, SHACL, SPARQL, and ontology-based traceability.

The goal of this artifact set is to show how semantic interoperability testing can be extended toward behavioral interoperability testing by checking whether observed runtime or simulated evidence conforms to expected scenario-level behavior.


## Repository structure

```text
Behavioral-Interoperability-Testing/
│
├── README.md
│
├── Behavioral Interoperability Testing Ontology (BITO)/
│   ├── README.md
│   ├── ontology/
│   ├── documentation/
│   ├── conceptual-diagram/
│   ├── competency-questions/
│   ├── sparql-dl-queries/
│   └── ontology-validation/
│       ├── oops!/
│       ├── hermit/
│       └── cq/
│
├── json-input-data/
│   ├── simulated-dataset-scenario-3.json
│   └── simulated-observed-evidence-scenario-3.json
│
├── rml-mappings/
│   ├── scenario-3-dataset-mapping.rml.ttl
│   └── scenario-3-observed-evidence-mapping.rml.ttl
│
├── rdf-graphs/
│   ├── dataset-graph.ttl
│   ├── observed-evidence-graph.ttl
│   ├── combined-validation-graph.ttl
│   └── s3-variants/
│       ├── v1-complete/
│       ├── v2-no-start-time/
│       ├── v3-no-acceptance/
│       └── v4-no-exec-start-ongoing/
│
├── shacl-shapes/
│   └── scenario-3-shacl-shapes.ttl
│
├── validation-results/
│   └── s3-variants/
│       ├── README.md
│       ├── v1-complete/
│       ├── v2-no-start-time/
│       ├── v3-no-acceptance/
│       └── v4-no-exec-start-ongoing/
│
└── technical-documentation/
    ├── Behavioral Interoperability Modeling Principles and Specification.docx
    ├── Behavioral Interoperability Testing Demonstration on the implemented use case.docx
    ├── Behavioral Rules, Mapping, and SHACL Shapes Catalog for the implemented use case.docx
    └── Solution Architecture Specification.docx
```

## Folder description

| Folder                                                 | Description                                                                                                                                                                                                 |
| ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Behavioral Interoperability Testing Ontology (BITO)/` | Contains the BITO ontology and ontology-level artifacts, including ontology files, generated documentation, conceptual diagrams, competency questions, SPARQL/DL queries, and ontology validation evidence. |
| `json-input-data/`                                     | Contains the JSON input files used in the implemented Scenario 3 workflow. One file represents the scenario input data, and the other represents observed evidence.                                         |
| `rml-mappings/`                                        | Contains the RML mapping rules used to transform the JSON input data and observed evidence into RDF graphs.                                                                                                 |
| `rdf-graphs/`                                          | Contains generated RDF graphs used as validation input. This includes the dataset graph, observed evidence graph, combined validation graph, and controlled Scenario 3 variant graphs.                      |
| `shacl-shapes/`                                        | Contains the SHACL shapes used to validate Scenario 3 behavioral rules. Some constraints use SHACL core features, while complex checks use embedded SPARQL constraints.                                     |
| `validation-results/` | Contains the validation outputs generated from the SHACL/SPARQL validation workflow. This folder includes the main validation artifacts and the Scenario 3 controlled evidence variant results. For each variant, the outputs include RDF validation result graphs, RDF trace graphs, visual report data, and human-readable HTML validation reports. |
| `technical-documentation/`                             | Contains technical documentation explaining the behavioral modeling principles, solution architecture, implemented use case, behavioral rules, RML mappings, and SHACL validation catalog.                             |

## Citation

If you use or refer to the artifacts in this repository, please cite the related paper:

```bibtex
@inproceedings{chy2026behavioralinteroperability,
  title     = {From Semantic to Behavioral Interoperability Testing: An Ontology-Driven Constraint Validation Framework},
  author    = {Chy, Tareq Md Rabiul Hossain and Bouter, Cornelis and Daniele, Laura and Kung, Antonio and Genest, Olivier and Lamboro, Henon Mengistu and Cornec, Léo and Rabrait, Cécile and Gyrard, Amélie},
  booktitle = {Proceedings of the SAGE Workshop 2026},
  year      = {2026}
}
```

The citation will be updated with the final proceedings details, DOI, page numbers, and publication URL once available.

## Funding acknowledgement

This work is prepared in the context of the HEDGE-IoT project, funded by the European Union's Horizon Europe research and innovation programme under Grant Agreement No. 101136216.


