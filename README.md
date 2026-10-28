# workshop-biomarker

- Workshop name: Biomarker Discovery : from theory to real world examples
- DDLS
- Duration: 3 days

This repository contains all the source code and assets (e.g. pictures)
for the training course materials.

## Files used by continuous integration scripts

<!-- markdownlint-disable MD013 --><!-- Tables cannot be split up over lines, hence will break 80 characters per line -->

Filename                                    |Description
--------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------
[`mlc_config.json`](mlc_config.json)        |Configuration of the link checker, use `markdown-link-check --config mlc_config.json --quiet docs/**/*.md` to do link checking locally
[`.spellcheck.yml`](.spellcheck.yml)        |Configuration of the spell checker, use [`./scripts/check_spelling.sh`](scripts/check_spelling.sh) to do spell check locally
[`.wordlist.txt`](.wordlist.txt)            |Whitelisted words for the spell checker, use [`./scripts/check_spelling.sh`](scripts/check_spelling.sh) to do spell check locally
[`.markdownlint.jsonc`](.markdownlint.jsonc)|Configuration of the Markdown linter, use [`./scripts/fix_markdown_style_errors.sh`](scripts/fix_markdown_style_errors.sh) to do markdown linting locally
[`.markdownlintignore`](.markdownlintignore)|Files ignored by the Markdown linter, use [`./scripts/fix_markdown_style_errors.sh`](scripts/fix_markdown_style_errors.sh) to do markdown linting locally

<!-- markdownlint-enable MD013 -->
