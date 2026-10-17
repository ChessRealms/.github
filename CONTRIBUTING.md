# Contributing to ChessRealms

Thank you for contributing to ChessRealms. Contributions of code,
documentation, tests, bug reports, and design feedback are welcome.

## Before you start

Read the target repository's README and any repository-specific contributing
guide. Repository-specific instructions take precedence over this organization
default.

For a significant feature, breaking change, or architectural change, open an
issue before starting implementation so the approach and scope can be agreed
on. Small fixes and documentation improvements can usually go directly to a
pull request.

## Make a change

1. Create a focused branch from the repository's default branch.
2. Keep the change limited to one logical purpose.
3. Add or update tests when behavior changes.
4. Update relevant documentation when commands, configuration, public APIs, or
   user-visible behavior change.
5. Run the validation commands documented by the target repository.
6. Open a pull request that explains the change and its motivation.

Do not commit credentials, personal data, editor state, build outputs, coverage
reports, or generated files unless the repository explicitly tracks them.

## Naming conventions

Use `<type>/<short-description>` for branch names. Common types are `feature`,
`fix`, `docs`, `test`, `refactor`, `perf`, `ci`, and `chore`.

Use Conventional Commit style for commit and pull request titles:

```text
<type>(<optional-scope>): <imperative summary>
```

Common title types are `feat`, `fix`, `docs`, `test`, `refactor`, `perf`, `ci`,
and `chore`. Examples:

```text
feat(editor): add FEN validation feedback
fix(engine): reject moves that expose the king
docs: clarify local development setup
```

## Pull requests

In the pull request description:

- explain what changed and why;
- link related issues when applicable;
- call out breaking changes, compatibility concerns, or notable risks;
- list the exact validation commands you ran and their results;
- state any validation you could not run and why;
- include screenshots or recordings for relevant visual changes.

Keep pull requests reviewable. Separate unrelated refactoring, formatting, and
dependency updates from behavioral changes whenever practical. Address review
feedback with additional commits; maintainers may squash commits when merging.

## Quality expectations

Follow the formatting, line-ending, and coding rules configured by the target
repository. Preserve backward compatibility unless the change explicitly calls
for a breaking release. New behavior should be covered by tests at the most
appropriate level, and all required continuous-integration checks should pass
before merge.
