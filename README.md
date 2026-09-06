# git-agent

## Project Overview

`git-agent` is a lightweight automation tool designed to simplify common Git workflows. It provides a set of commands for managing branches, commits, and pull requests directly from the command line, allowing developers to streamline their development process.

## Features

- Create, switch, and delete branches
- Stage, commit, and amend changes
- Open pull requests with pre-filled templates
- Interactive prompts for common Git operations
- Extensible plugin architecture

## Installation

### Prerequisites

- Python 3.8 or newer
- Git 2.20+ installed and available in your PATH

### Using pip

```bash
pip install git-agent
```

### From source

```bash
# Clone the repository
git clone https://github.com/yourusername/git-agent.git
cd git-agent

# Install dependencies
pip install -r requirements.txt

# Install the package in editable mode
pip install -e .
```

## Usage Examples

### Basic Commands

```bash
# Initialize a new git-agent repository (if needed)
git-agent init

# Create and switch to a new feature branch
git-agent branch create feature/login

# Stage all changes and commit with a message
git-agent commit -m "Add login feature"

# Push the current branch and open a PR
git-agent pr create --title "Login Feature" --description "Implements user login"
```

### Interactive Mode

```bash
# Run git-agent in interactive mode to be guided through common tasks
git-agent interactive
```

## Configuration

`git-agent` can be configured via a `git-agent.toml` file placed in the root of your repository. Example configuration:

```toml
[default]
branch = "main"
remote = "origin"

[pr]
template = "templates/pr_template.md"
```

## Contribution Guidelines

We welcome contributions! Please follow these steps:

1. **Fork the repository** and clone your fork.
2. **Create a new branch** for your feature or bug fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Write tests** for new functionality.
4. **Run the test suite** to ensure everything passes:
   ```bash
   pytest
   ```
5. **Commit your changes** with clear commit messages.
6. **Push** to your fork and open a pull request.

### Code Style

- Follow PEP 8 guidelines.
- Use type hints where appropriate.
- Run `black` and `ruff` before committing.

### Reporting Issues

If you encounter any bugs or have feature requests, please open an issue on the GitHub repository with a clear description and steps to reproduce.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

*Happy coding!*