# Hello World Python Project

## Project Overview

This repository contains a simple Python project that demonstrates a basic "Hello, World!" application. It serves as a minimal example for setting up a Python package, including project structure, a simple script, and the necessary configuration files (`pyproject.toml`, `uv.lock`). The goal is to provide a clean starting point for developers who want to create new Python projects or learn about packaging, testing, and documentation practices.

## Installation

### Prerequisites

- Python 3.9 or newer
- [uv](https://github.com/astral-sh/uv) (recommended) or `pip`

### Using `uv`

```bash
# Install uv if you don't have it
curl -LsSf https://astral.sh/uv/install.sh | sh

# Install the project in editable mode
uv sync --dev
```

### Using `pip`

```bash
# Create a virtual environment (optional but recommended)
python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\\Scripts\\activate`

# Install the package in editable mode
pip install -e .
```

## Usage

After installation, you can run the provided script directly from the command line:

```bash
python -m hello
```

Or, if you installed the package, you can use the entry point:

```bash
hello
```

Both commands will output:

```
Hello, World!
```

### Running the `main` function programmatically

```python
from hello import main

if __name__ == "__main__":
    main()
```

## Contributing

We welcome contributions! Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for details on how to get started, our coding standards, and the process for submitting pull requests.

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.