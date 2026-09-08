# DataBounty Datasets

This repository is DataBounty's GitHub catalogue of published community datasets. Each dataset has its own
folder under [`datasets/`](datasets/), with a human-readable description, a machine-readable manifest, its
license, and the public training/evaluation items.

The same released data is also available on Hugging Face. GitHub is the browsable source and version history;
Hugging Face is the primary distribution endpoint for dataset tooling and large-file access.

## Published datasets

| Dataset | Public contributor items | GitHub folder | Hugging Face |
|---|---:|---|---|
| Python Execution Trace & Output Prediction | 1,000 | [Open folder](datasets/python-execution-trace-output-prediction-cmskdimp/) | [Open dataset](https://huggingface.co/datasets/databounty-io/python-execution-trace-output-prediction-cmskdimp) |
| Python Data Transformation Scripts | 1,000 | [Open folder](datasets/python-data-transformation-scripts-cmskdijz/) | [Open dataset](https://huggingface.co/datasets/databounty-io/python-data-transformation-scripts-cmskdijz) |
| Extract Metrics from Log Fixtures | 1,000 | [Open folder](datasets/extract-metrics-from-log-fixtures-cmskdlip/) | [Open dataset](https://huggingface.co/datasets/databounty-io/extract-metrics-from-log-fixtures-cmskdlip) |

## Repository layout

```text
datasets/
  <dataset-slug>/
    README.md          Dataset purpose, scope, contributors, and licence
    data/items.jsonl   One accepted contributor item per line
    manifest.json      Provenance, counts, schema, and release metadata
    LICENSE            Licence for that dataset
```

`data/items.jsonl` contains accepted contributor items only. Sponsor reference examples, unpublished uploads,
review evidence, credentials, and application code are never stored in this repository.

`manifest.json` is the authoritative machine-readable record for a release. It includes the release count,
dataset contract, contributor attribution, licence, and integrity metadata. The publication pipeline keeps the
JSONL and manifest aligned with the matching Hugging Face release once both provider pushes have completed.

## How publication works

DataBounty publishes a dataset only after its items have completed validation, review, and publication approval.
The publication service writes only the affected `datasets/<dataset-slug>/` folder, so publishing or retracting
one dataset does not modify the others. Retraction removes that folder in a normal Git commit, preserving an
auditable history.

## Contributing

Contributions are submitted and reviewed through DataBounty, not through pull requests to this repository.
Each published dataset folder credits the contributors included in that release. To report a metadata error,
licensing concern, broken link, or withdrawal request, open an issue without including private data,
credentials, or unpublished material.

For publication or repository questions, contact [DataBounty](mailto:cipher@databounty.io).

## Security and scope

This repository is for released dataset artifacts only. Do not commit access tokens, personal data, unpublished
submissions, or application configuration. Publication credentials belong only in the API deployment's secret
manager.
