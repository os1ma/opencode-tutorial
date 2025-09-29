# Agent Guidelines for Python Project Template

## Build/Test/Lint Commands
- **Install dependencies**: `uv sync`
- **Type checking**: `uv run mypy .`
- **Linting**: `uv run ruff check .`
- **Format code**: `uv run ruff format .`
- **Run single test**: No test framework configured yet
- **Build requirements**: `make` or `uv export -o requirements.txt`

## Code Style Guidelines
- **Python version**: >=3.11 (see pyproject.toml)
- **Type hints**: Strict mypy enabled - always add type hints
- **Linting**: Ruff with "ALL" rules enabled, specific ignores for documentation (D), annotations (ANN), try/except (TRY), error messages (EM), future annotations (FA), and others
- **Import style**: Follow ruff formatting
- **Error handling**: Avoid bare except clauses, use specific exceptions
- **Naming**: Follow PEP 8 conventions
- **Dependencies**: Use `uv add <package>` to add new dependencies
- **File structure**: Keep project minimal and organized

## Notes
- No existing Cursor rules or Copilot instructions found
- This is a template project with minimal structure
- Always run `uv run mypy .` and `uv run ruff check .` before committing