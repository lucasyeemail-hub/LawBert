# LawBERT

LawBERT is an early project for helping people understand long documents before they sign or respond. The intended users are ordinary people who need a readable explanation of a document’s sections, costs, dates, obligations, and cancellation terms, with each explanation connected to the exact original passage.

## Status

This workspace currently contains project documentation only. No application code, framework, dependency manifest, tests, or prior Git history was present when inspected; a local Git repository has now been initialized to track this setup. The product is not implemented, tested with users, or validated for legal reliability.

## Planned MVP

- Accept a user-provided document and extract readable text.
- Explain the document section by section in plain language.
- Surface important costs, dates, obligations, and cancellation terms.
- Link each explanation to its exact source passage.
- Clearly flag unreadable text and uncertain interpretations.

The product should support understanding, not provide legal advice or tell someone whether to sign.

## Technology

No implementation stack or legal-domain BERT checkpoint is specified in the files available in this workspace. “LawBERT” is the project name; it does not identify a particular model. Model choice and any model-assisted tasks remain open decisions. Do not treat BERT as a conversational assistant or as a source of reliable legal advice.

## Local setup

There is no application to install or run yet. To work on the documentation, clone the repository once it has a remote configured, or open this directory directly. See [docs/setup.md](docs/setup.md) for current state, future setup guidance, and troubleshooting.

Basic documentation checks can be run with:

```sh
git status --short
```

Application run, lint, and test commands will be documented when the corresponding framework and code are added.

## Product and setup notes

- [Product overview](docs/product-overview.md)
- [Setup and troubleshooting](docs/setup.md)
