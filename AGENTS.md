# Agent Instructions for python-terraform-bridge

## Overview

This package bridges Python classes to Terraform external data sources and modules.

## Before Starting

```bash
cat memory-bank/activeContext.md
```

## Development Commands

```bash
# Install dependencies
uv sync --extra tests

# Run tests
uv run pytest tests/ -v

# Lint
uvx ruff check src/ tests/
uvx ruff format src/ tests/

# Build
uv build
```

## Commit Messages

Use conventional commits:
- `feat(bridge): new feature` → minor
- `fix(bridge): bug fix` → patch

## Quality Standards

- All tests must pass
- Use absolute imports (`from python_terraform_bridge...`)
- Include `from __future__ import annotations`
- Type hints required
