# 📦 spellborne-data

**CLI & Python API to scrape monsters & moves from Spellborne.**

![PyPI](https://img.shields.io/pypi/v/spellborne-data)
![Build](https://img.shields.io/github/actions/workflow/status/yourusername/spellborne-data/ci.yml)
![Coverage](https://img.shields.io/codecov/c/github/yourusername/spellborne-data)

## Features

* Scrape monster data (stats, abilities) from Spellborne.
* Extract and format move lists with attributes.
* Output results in JSON or CSV for easy integration.
* Simple, intuitive CLI plus full Python module for custom workflows.

## Installation

```bash
git clone https://github.com/yourusername/spellborne-scraper.git
cd spellborne-scraper
pip install .
```

## Usage

### CLI

```bash
# Scrape all monsters to JSON\sspellborne-scraper scrape monsters --output monsters.json
# Scrape moves to CSV\sspellborne-scraper scrape moves --output moves.csv
```

### Python API

```python
from spellborne_scraper import monsters, moves

# Get list of monster dicts
data = monsters.fetch_all()
# Get move details
move_list = moves.fetch_all()
```

## Tests

```bash
pytest tests/
```

## License

MIT · [License](LICENSE)
