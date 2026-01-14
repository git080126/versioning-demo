# Versioning Demo

This repository demonstrates a simple and practical Git-based branching and versioning strategy for managing multiple environments.

## Purpose
The goal of this repository is to show:
- How code flows across environments using Git branches
- How versioning can be handled using Git tags
- How PR-based merging enforces control and review

This is a demo repository created for understanding and discussion.

## Branch Structure
The repository follows an environment-based branching model:

- `dev`   → Development work
- `uat`   → User Acceptance Testing
- `demo`  → Demo / validation
- `main`  → Production (final)

## Flow
Code promotion happens in the following order:
dev → uat → demo → main
Each promotion is expected to happen via Pull Requests.

## Versioning
Releases are identified using Git tags following semantic versioning:

Examples:
- `v1.0.0` → Initial release
- `v1.0.1` → Bug fix
- `v1.1.0` → New feature

Tags represent stable snapshots of the code.

## Pull Request Rules
- Direct merges are not allowed
- Every branch requires a Pull Request
- At least one approval is required before merging

## Notes
- This repository does not include CI/CD or Docker setup
- The focus is purely on Git flow and versioning concepts
- Created for demonstration and learning purposes
