# Contributing to Urekz repositories

## Source of work

Planned work lives in Plane. GitHub Issues are not the work-management system for Urekz repositories.

## Branches

Use short-lived branches from `main`:

`<type>/<PLANE-ID>-<short-description>`

Examples:

- `feat/UCODE-42-semantic-memory`
- `fix/EMR-27-mobile-layout`
- `docs/UCODE-61-agent-model`

Exceptional maintenance with no Plane item may use:

`chore/maintenance-<short-description>`

and the Pull Request must explicitly state `N/A - maintenance exception`.

## Commits

Use Conventional Commits. Human commits should be signed using the contributor's configured signing method.

## Pull Requests

Normal changes reach `main` through a Pull Request. Every PR requires human review by a person other than its author before merge.

CI must be green before merge. Resolve review conversations before merge.

## Merge strategy

Use Squash Merge only. The Pull Request title becomes the final commit title on `main`, so PR titles must use Conventional Commit syntax.
