# Contributing

Thank you for considering contributing to this project!

## How to Contribute

### Reporting Bugs

- Check if the bug has already been reported in [Issues](../../issues)
- If not, create a new issue with a clear title and description
- Include steps to reproduce the bug
- Include expected vs actual behavior

### Suggesting Features

- Check if the feature has already been suggested in [Issues](../../issues)
- Create a new issue describing the feature and why it would be useful

### Submitting Pull Requests

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature-name`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some feature'`)
5. Push to the branch (`git push origin feature/your-feature-name`)
6. Open a Pull Request

### Code Style

This project uses automated code quality tools. Please ensure your code passes all checks:

1. **Set up pre-commit hooks** (first time only):
   ```bash
   uv pip install pre-commit
   pre-commit install
   ```

2. **Run code quality checks**:
   ```bash
   # Run all pre-commit hooks
   pre-commit run --all-files

   # Or run tools individually
   ruff check .          # Linting
   ruff format .         # Formatting
   pylint your_module/   # Code analysis
   ```

3. **Code style guidelines**:
   - Follow PEP 8 style guidelines
   - Use type hints where appropriate
   - Write docstrings for functions and classes
   - Keep line length to 100 characters (configured in pyproject.toml)
   - Use `.editorconfig` settings for consistent formatting

4. **Pre-commit hooks will automatically**:
   - Format code with Ruff
   - Check for common issues
   - Validate YAML, TOML, and JSON files
   - Remove trailing whitespace
   - Ensure files end with a newline

### Code of Conduct

Please note that this project has a [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
