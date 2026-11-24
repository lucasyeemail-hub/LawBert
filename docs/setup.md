# Setup and troubleshooting

## Current project contents

This checkout contains documentation only. Inspection found no application source, package/dependency manifest, framework configuration, tests, environment variable usage, or prior Git history. A local Git repository is now initialized, with no commits or remote configured. As a result, there are no truthful install, app-run, lint, or test commands to provide yet. This guide records the current state rather than guessing a stack.

## Prerequisites

For the current documentation-only checkout:

- Git, if working from a clone or checking repository status.
- A text editor.

There are no runtime prerequisites for the application because no application has been added.

## Installation

No dependency installation is currently required. Once an application framework is selected, add its exact runtime version and package-manager commands here, based on the checked-in dependency files.

## Configuration

No configuration variables are currently required, so there is no `.env.example`. When configuration is introduced, document each variable and commit only safe placeholders. Never commit credentials, API keys, model weights, or real user documents.

## Run

There is no application command to run yet. For a documentation-only checkout, inspect repository state with:

```sh
git status --short
```

Document the actual development server command here when app code and its manifest are added.

## Development commands

No formatter, linter, or test runner is configured. Do not assume a command such as `npm test` or `pytest` until that tool is part of the project. Add commands here when they exist and confirm them against the checked-in files.

## Troubleshooting

- **I expected app code:** confirm that the correct LawBERT project directory or branch is open. This checkout had no source files at setup time.
- **I need a model:** no checkpoint is selected or configured. Choosing one requires a documented task, evaluation plan, license review, and a decision about whether it is suitable for the MVP.
- **I need a GitHub remote:** none was configured in this workspace. This setup does not create or push to a remote. Choose the repository name and visibility before creating one.
- **I have private documents or model files:** keep them outside Git. The `.gitignore` excludes common local environment files, model artifacts, and document samples.
