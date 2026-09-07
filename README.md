# ft-data-prep-lab

Clean and split JSONL datasets for fine-tuning

## Features

- Length filters keep the sweet spot
- Dedup by normalized instruction text
- Deterministic split with a seed
- Prints a stats summary you can eyeball

## Usage

```bash
python prep.py raw.jsonl --out-dir data/ --valid-ratio 0.1
```

## Getting started

```bash
# stdlib only
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
└── prep.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
