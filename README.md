# DataBounty Datasets

This private repository is the destination for datasets published by DataBounty. It does not store
application code, unpublished uploads, publication jobs, or credentials.

## Where datasets are published

- **Hugging Face** is the primary dataset host and supports larger files through Git LFS.
- **GitHub** (here) holds every published dataset as its own folder under `datasets/<slug>/`, inside this
  one shared repository — not as a separate repository per dataset.

A publish only touches its own dataset's folder (an overlay commit onto the existing tree), so one dataset
publishing never affects any other dataset's folder here. A retraction removes just that dataset's folder as
a commit — the repository's own visibility is a separate, one-time operator decision, never something a single
dataset's publish or retraction flips.

## Published datasets

No datasets have been published to this repository yet. When they are, each will appear as
`datasets/<slug>/`, containing `data/items.jsonl`, `manifest.json`, and a dataset-card `README.md` — the same
provenance and license metadata as its Hugging Face counterpart.

## Publication policy

A dataset is listed only after validation, human review, publication approval, and confirmation from the
destination provider. Pending, failed, unconfigured, and withdrawn destinations retain their precise status.
Withdrawal removes public access while preserving the publication history.

Do not commit personal data, access tokens, or unpublished material here beyond what the publication pipeline
itself writes. Provider credentials belong in the API deployment's secret manager, not in this repository or
its GitHub environment.

## Reporting an issue

Use this repository's issues to report incorrect metadata, licensing concerns, broken provider links, or a
required withdrawal. Do not include private data, credentials, or unpublished dataset content in an issue.
