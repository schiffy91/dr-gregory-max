---
applyTo: "**/*.py"
---
# Coding Standards

## Principles
KISS, YAGNI, SRP. Simple > Complex. Modular with clear interfaces.

## Size Limits
| Metric | Limit |
|--------|-------|
| File | 300 lines |
| Function | 50 lines |
| Class | 200 lines |

## Code Style
- **Python**: PEP 8, type hints, 100 char limit

## Dependencies (CRITICAL)
**NEVER** run `pip/apt/npm install` directly.

Declare in manifests first:
- Python: root `requirements.txt` (single consolidated file)
- System: `.devcontainer/Dockerfile`

## Version Control
- **Commit Granularity**: Commit often. Avoid "Initial commit" dumps.
- **Structure**: Commit after each logical step (e.g., "Add HTML structure", "Add basic CSS", "Refine typography").
- **Messages**: Use imperative mood ("Add feature" not "Added feature").
