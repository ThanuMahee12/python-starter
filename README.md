# Python Starter Template

A modern Python project template with uv, pre-commit hooks, ruff, and pylint for code quality and formatting.

## Features

- **UV Package Manager**: Fast, modern Python package management
- **Pre-commit Hooks**: Automated code quality checks before commits
- **Ruff**: Lightning-fast Python linter and formatter
- **Pylint**: Comprehensive Python code analysis
- **GitHub Actions**: Pre-configured CI/CD workflow
- **Code Quality**: Best practices for Python development

## Quick Start

### Prerequisites

- Python 3.9 or higher
- [uv](https://github.com/astral-sh/uv) package manager

### Installation

1. Use this template to create a new repository on GitHub

2. Clone your new repository:
```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
```

3. Install uv (if not already installed):
```bash
# On macOS and Linux
curl -LsSf https://astral.sh/uv/install.sh | sh

# On Windows
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

4. Create and activate a virtual environment:
```bash
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

5. Install pre-commit hooks:
```bash
uv pip install pre-commit
pre-commit install
```

### Configuration

1. Update `pyproject.toml` with your project details:
   - Change `name` to your project name
   - Update `description`
   - Add your author information
   - Add your project dependencies

2. Customize tool configurations in `pyproject.toml`:
   - Ruff settings (linting and formatting)
   - Pylint rules
   - Other tool configurations as needed

## Usage

### Adding Dependencies

```bash
# Add a runtime dependency
uv pip install package-name

# Add a development dependency
uv pip install --dev package-name
```

### Running Code Quality Checks

```bash
# Run ruff linter
ruff check .

# Run ruff formatter
ruff format .

# Run pylint
pylint your_module/

# Run all pre-commit hooks manually
pre-commit run --all-files
```

### Pre-commit Hooks

Pre-commit hooks automatically run on every commit. They include:
- Ruff linting and formatting
- Pylint code analysis
- Trailing whitespace removal
- End of file fixing
- YAML, TOML, and JSON validation
- Large file detection
- Private key detection

## Project Structure

```
.
├── .github/
│   └── workflows/          # GitHub Actions workflows
├── .pre-commit-config.yaml # Pre-commit configuration
├── pyproject.toml          # Project metadata and tool configuration
├── .gitignore              # Git ignore rules
├── README.md               # This file
├── LICENSE                 # Project license
├── CONTRIBUTING.md         # Contribution guidelines
├── CODE_OF_CONDUCT.md      # Code of conduct
└── SECURITY.md             # Security policy
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to contribute to this project.

## Code of Conduct

This project adheres to a [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## Security

For security concerns, please see [SECURITY.md](SECURITY.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
