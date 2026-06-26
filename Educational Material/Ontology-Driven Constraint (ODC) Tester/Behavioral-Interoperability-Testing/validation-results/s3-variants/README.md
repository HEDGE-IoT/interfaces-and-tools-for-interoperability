# Scenario 3 Controlled Evidence Variants

This folder contains the validation outputs for four controlled evidence variants derived from Flexible Start use case Scenario 3.

Each variant uses the same scenario-derived behavioral rules but changes the available evidence in order to test whether the validation workflow can distinguish compliant behavior, missing evidence, non-conforming behavior, and skipped validation steps.

## Variant folders

| Folder | Variant | Expected validation behavior |
|---|---|---|
| `v1-complete/` | Complete evidence | All behavioral steps pass. |
| `v2-no-start-time/` | Missing requested start-time evidence | Step 1 becomes inconclusive and later steps are skipped. |
| `v3-no-acceptance/` | Missing acceptance evidence | Step 2 becomes inconclusive and Step 3 is skipped. |
| `v4-no-exec-start-ongoing/` | Missing execution-start evidence and ongoing final status | Step 1 and Step 2 pass; Step 3 contains inconclusive and failed outcomes. |

## Files in each variant folder

Each variant folder may contain:

- `validation-results-graph.ttl`: machine-readable validation result graph
- `rdf-trace-graph.ttl`: RDF trace graph linking evidence, rules, and verdicts
- `visual-report-data.json`: JSON data used to generate the visual report
- `behavioral-validation-report.html`: human-readable validation report