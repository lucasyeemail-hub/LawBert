# Product overview

## User problem

People may need to sign or respond to long documents whose language, structure, or length makes important details hard to find. They need help understanding what the text says, including costs, dates, obligations, and cancellation terms, while being able to verify an explanation against the original wording.

## Intended users

The intended users are ordinary people reviewing documents for themselves. The product is meant to improve comprehension and navigation; it is not a lawyer, a legal representative, or a decision-maker.

## Proposed workflow

1. A user uploads or otherwise provides a document.
2. The app extracts text and communicates when portions are unreadable or uncertain.
3. The app presents a plain-language explanation section by section.
4. Important costs, dates, obligations, and cancellation terms are highlighted.
5. Each explanation can be checked against the exact passage in the source document.

This is a proposed MVP, not implemented behavior. The workspace contains no app code yet.

## Privacy expectations

Documents may contain sensitive personal or financial information. The product should minimize collection and retention, explain where documents and extracted text are processed, restrict access, and avoid using user documents for model training without explicit informed consent. The storage, processing, deletion, and retention design is not yet specified. Until it is, do not commit real documents, extracted text, or credentials to the repository.

## Limitations and safety

- Explanations can be incomplete or wrong; users should be able to inspect the cited source passage.
- Poor scans, OCR errors, missing pages, ambiguous language, and unsupported formats can reduce accuracy. The app should say when text or interpretation is uncertain rather than conceal it.
- The product should help users understand document text. It should not advise whether to sign, provide legal advice, or imply that a model can reliably resolve legal questions.
- No legal-domain BERT checkpoint is specified in this workspace. “LawBERT” alone does not identify a model. If a checkpoint is later selected, document its exact source, intended task, license, evaluation evidence, and limits. A BERT encoder/classifier should not be presented as a conversational assistant or legal-advice generator.
- The project has no implementation or user-validation evidence in the inspected workspace.

## Decisions still to be made

- Which document types, file formats, languages, and maximum sizes will the MVP support?
- How will text extraction and OCR work, and how will source passages remain aligned with explanations?
- Will explanations use a language model, deterministic rules, or a combination? Which model/service, if any, is acceptable?
- If a legal-domain BERT checkpoint is considered, what specific task will it perform (for example, classification), and what evidence will establish suitability?
- Where will processing and storage occur? What are the retention, deletion, access-control, and consent policies?
- How will uncertainty be detected and shown to users?
- How will quality, accessibility, and user comprehension be evaluated without implying legal reliability?
- Which framework, deployment target, and development workflow will the project use?
