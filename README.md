# mlp-sandbox-x

Minimal training loop I use to test ideas fast

## Highlights

- Single file model definition, easy to hack
- Gradient clipping and clean metrics logging
- Metrics logged to CSV for plotting
- Cosine LR schedule with warmup
- Synthetic dataset mode: no download needed to smoke-test

## Usage

```bash
python train.py --epochs 5 --synthetic
# metrics land in runs/metrics.csv
```

## Installation

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   └── usage.md
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── LICENSE
├── model.py
├── requirements.txt
└── train.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

## License

MIT - see [LICENSE](LICENSE).
