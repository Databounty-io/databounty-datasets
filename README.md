# DataBounty Datasets

> Open, community-built coding datasets — released with clear provenance, licensing, and contributor credit.

[DataBounty](https://databounty.io) is a community programme for building useful datasets. This repository is the public GitHub catalogue for released dataset artifacts. For browsing and large-file tooling, each release is also available on [Hugging Face](https://huggingface.co/databounty-io).

## What is published

Every dataset folder contains only the artifacts approved for that release:

- accepted contributor items;
- a human-readable dataset card;
- a machine-readable manifest with counts, provenance, licence, and attribution metadata; and
- the dataset's licence text when it is bundled.

Sponsor reference material, unpublished submissions, review evidence, credentials, personal data, and application code are never published here.

## Published datasets

| Dataset | Released contributor items | GitHub | Hugging Face |
|---|---:|---|---|
| Python Execution Trace & Output Prediction | 1,000 | [Browse files](datasets/python-execution-trace-output-prediction-cmskdimp/) | [Open dataset](https://huggingface.co/datasets/databounty-io/python-execution-trace-output-prediction-cmskdimp) |
| Python Data Transformation Scripts | 1,000 | [Browse files](datasets/python-data-transformation-scripts-cmskdijz/) | [Open dataset](https://huggingface.co/datasets/databounty-io/python-data-transformation-scripts-cmskdijz) |
| Extract Metrics from Log Fixtures | 1,000 | [Browse files](datasets/extract-metrics-from-log-fixtures-cmskdlip/) | [Open dataset](https://huggingface.co/datasets/databounty-io/extract-metrics-from-log-fixtures-cmskdlip) |

## Repository layout

```text
datasets/
  <dataset-slug>/
    README.md          Purpose, scope, source notes, and contributor credits
    data/items.jsonl   One accepted contributor item per line
    manifest.json      Release metadata, counts, provenance, and integrity fields
    LICENSE            Licence for this dataset, where bundled
```

### Using a release

- Read the dataset folder's `README.md` before use; its stated licence and scope apply to that release.
- Use `data/items.jsonl` as the released item stream. Each line is one JSON object.
- Treat `manifest.json` as the authoritative machine-readable release record. It records the accepted-item count, dataset contract, contributor-credit policy, licence, and release metadata.
- Use the matching Hugging Face dataset for common dataset-tooling workflows and larger-file access.

## Release and correction policy

DataBounty publishes only release-approved community artifacts. A release is folder-scoped: adding, correcting, or retracting one dataset never replaces another dataset's files.

If you find a metadata error, licensing concern, broken link, or need to request a correction or withdrawal, please [open an issue](https://github.com/Databounty-io/databounty-datasets/issues/new) without including credentials, private data, or unpublished material.

Contributions are submitted and reviewed through [DataBounty](https://databounty.io), not through pull requests to this catalogue repository.

## Security and privacy boundary

This repository is intentionally limited to released dataset artifacts. Do not commit access tokens, application configuration, unpublished submissions, or personal data. Publication credentials are held only by DataBounty's deployment secret manager.

Questions about a release or this catalogue: [cipher@databounty.io](mailto:cipher@databounty.io).
