# MLOps Zoomcamp

This repository contains my work for the [MLOps Zoomcamp](https://github.com/DataTalksClub/mlops-zoomcamp) by DataTalks.Club.

## Getting Started

### Prerequisites

- Python 3.11 or 3.12
- [uv](https://github.com/astral-sh/uv) (for dependency management)
- `make`

### Installation

To set up the development environment and install all dependencies:

```bash
make deps
```

This will create a virtual environment and install all necessary packages, including development and notebook dependencies.

## Development

The project uses a `Makefile` to simplify common tasks:

- **Install dependencies:** `make deps`
- **Run tests:** `make test`
- **Run linter and formatter (Ruff):** `make lint`
- **Run static checks:** `make check`
- **Clean project artifacts:** `make clean`
- **Run all checks (clean, lint, test, license):** `make all`

## Notebooks

To work with Jupyter notebooks, you can start Jupyter Lab:

```bash
uv run jupyter lab
```

## Testing

Tests are managed using `pytest`. You can run the test suite with:

```bash
make test
```

For non-deterministic tests:

```bash
make test-flaky
```
