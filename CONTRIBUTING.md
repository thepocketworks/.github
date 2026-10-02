<!-- # links ------------------------------------------------------------- # -->

[conventionalcommits]: https://www.conventionalcommits.org/

<!-- # introduciton ------------------------------------------------------ # -->

## Contributing to This Project

Thank you for your interest in contributing to this project.

I believe open-source works best when people can collaborate in a
simple, clear, and respectful way. Contributions of all kinds are
welcome, whether they are bug fixes, improvements, documentation, tests,
feature proposals, or other ideas that can make the project better.

Before contributing, please take a moment to read this document. It
explains the development workflow, commit conventions, and
expectations for contributions.

By contributing to this project, you agree to follow the project's
[**Code of Conduct**](./CODE_OF_CONDUCT.md).

<!-- # before contributing ----------------------------------------------- # -->

## Before You Start

Before working on a contribution, please consider checking the existing:

- Issues.
- Pull requests.
- Discussions.
- Documentation.
- Project roadmap, when available.

This helps avoid duplicated work and makes it easier to understand the
current direction of the project.

For significant changes, especially new features or architectural
changes, it is recommended to discuss the idea before starting
implementation.

Small bug fixes, documentation improvements, tests, and other
straightforward contributions can usually be submitted directly.

<!-- # issues ------------------------------------------------------------ # -->

## Issues

> [!WARNING]\
> **Do not use public Issues to report security vulnerabilities.**\
> Security vulnerabilities should be reported privately according to
> the project's [Security Policy](./SECURITY.md).

Issues are primarily intended for:

- Bug reports.
- Feature requests.
- Improvements.
- Documentation problems.
- Questions or other non-sensitive project discussions.

Before opening a new issue, please search the existing issues to make
sure the topic has not already been reported or discussed.\
Please provide enough context for others to understand and reproduce
the problem.

For bug reports, useful information may include:

- What you expected to happen.
- What actually happened.
- Steps to reproduce the problem.
- Relevant error messages.
- Project version.
- Operating system.
- Runtime or tool versions.
- A minimal reproduction, when possible.

<!-- # development setup ------------------------------------------------- # -->

## Development Setup

Before making changes, set up the project locally according to the
instructions provided in the project documentation.

A typical contribution workflow is:

1. Fork the repository.
2. Clone your fork.
3. Create a dedicated branch for your changes.
4. Install the project dependencies.
5. Make your changes.
6. Run the relevant tests and checks.
7. Commit your changes using the project's commit convention.
8. Push your branch to your fork.
9. Open a Pull Request.

Keep your changes focused.\
A Pull Request should ideally address one problem or one clearly
related group of changes.

<!-- # branches ---------------------------------------------------------- # -->

## Branches

Please create a separate branch for each contribution.\
Use descriptive branch names that make the purpose of the branch clear.

Examples:

```zsh
feature/add-plugin-system         # feature
fix/windows-path-resolution       # fix
docs/improve-installation-guide   # docs
refactor/simplify-config-loader   # refactor
test/add-parser-coverage          # test
```

Avoid working directly on the default branch.\
Keeping contributions isolated makes reviews easier and helps maintain
a clean project history.

<!-- # code quality ------------------------------------------------------ # -->

## Code Quality

Contributions should follow the existing conventions and architecture
of the project.\
Before submitting a Pull Request:

- Keep the implementation simple and focused.
- Follow the existing code style.
- Avoid unrelated changes.
- Add or update tests when appropriate.
- Update documentation when behavior changes.
- Remove unnecessary debug code.
- Make sure existing functionality is not unintentionally broken.
- Run the available linting, formatting, type-checking, and
  test commands.

If the project already provides automated formatting or linting tools,
use them instead of manually applying a different style.\
Consistency is generally more valuable than introducing a new style
for a single contribution.

<!-- # commits ----------------------------------------------------------- # -->

## Commit Convention

This project uses [Conventional Commits][conventionalcommits] to keep
the Git history clear, consistent, and easy to understand.\
A commit message should follow this structure:

```zsh
<type>[optional scope]: <description>
```

For example:

```zsh
feat: add plugin system
fix: resolve Windows path handling
docs: improve installation guide
test: add parser coverage
refactor: simplify configuration loading
```

### Commit Types

The following commit types should be used when applicable:

| Type     | Description                                                      |
| -------- | ---------------------------------------------------------------- |
| `feat`   | Introduces a new feature or user-facing capability.              |
| `fix`    | Fixes a bug.                                                     |
| `docs`   | Changes documentation only.                                      |
| `style`  | Changes formatting or style without changing behavior.           |
| `pef`    | Improves performance.                                            |
| `test`   | Adds or updates tests.                                           |
| `build`  | Changes the build system or dependencies.                        |
| `ci`     | Change Continous Integration configuration.                      |
| `chore`  | Maintenance changes that do not affect the application directly. |
| `revert` | Reverts a previous commit.                                       |

Use the type that best describes the purpouse of the change.

### Commit Descriptions

Commit descriptions should be:

- Clear and concise.
- Written in the imperative style.
- Focused on what the commit changes.
- Specific enough to understand without reading the entire diff.

Prefer:

```zsh
feat: add configuration validation
```

Instead of:

```zsh
added some validation stuff
```

Avoid unnecessary punctuation or vague descriptions such as:

```zsh
fix: changes
update: stuff
chore: miscellaneous improvements
```

### Scopes

Scopes are optional and should be used when they make the commit
easier to understand.\
For example:

```zsh
feat(cli): add project initialization command
fix(parser): handle empty input
docs(api): improve authentication examples
test(core): cover configuration loading
```

Use scopes that are meaningful within the project.\
Do not introduce scopes simply for these sake or having one.

### Breaking Changes

It a commit introduces a breaking change, indicate it by adding `!`
after the type or scope:

```zsh
feat!: remove legacy configuration format
```

or:

```zsh
feat(api)!: change authentication interface
```

Breaking changes should also include a `BREAKING CHANGE:` footer when
additional migration information is useful:

```zsh
feat(api)!: change authentication interface

BREAKING CHANGE: authentication now requires an explicit client configuration.
```

Breaking changes should be clearly explained in the Pull Request as well.

<!-- # commit examples --------------------------------------------------- # -->

## Commit Examples

Good commit messages include:

```zsh
feat: add project initialization command
```

```zsh
feat(cli): add interactive configuration
```

```zsh
fix: prevent duplicate event handlers
```

```zsh
fix(parser): handle empty configuration files
```

```zsh
docs: improve contribution guide
```

```zsh
test: add coverage for configuration parser
```

```zsh
refactor(core): simplify dependency resolution
```

```zsh
perf: reduce startup time
```

```zsh
ci: update release workflow
```

<!-- # atomic committs --------------------------------------------------- # -->

## Keep Commits Focused

Whenever practical, each commit should represent one logical change.\
Avoid combining unrelated changes into the same commit.

For example, instead of:

```zsh
feat: add authentication, fix parser, update docs and change CI
```

prefer separate commits when the changes are genuinely independent:

```zsh
feat(auth): add authentication support
fix(parser): handle malformed input
docs: update authentication guide
ci: update test workflow
```

Focused commits make code review, debugging, reverting, and future
maintenance easier.

<!-- # pull requests ----------------------------------------------------- # -->

## Pull Requests

When your changes are ready, open a Pull Request against the appropriate
default branch.\
A good Pull Request should explain:

- What was changed.
- Why the change was necessary.
- How the change works, when relevant.
- How the change was tested.
- Any limitations or known issues.
- Whether the change introduces breaking behavior.

Keep the Pull Request focused on the related changes.\
If a Pull Request becomes too large or starts covering unrelated topics,
consider splitting it into smaller contributions.

### Pull Request Title

Pull Request titles should follow the same
[Conventional Commits][conventionalcommits] format as commit messages.\
Examples:

```zsh
feat: add plugin system
```

```zsh
fix: resolve configuration loading issue
```

```zsh
docs: improve installation documentation
```

```zsh
refactor(chore): simplify dependency resolution
```

This makes the project's contribution history easier to understand and keeps
Pull Requests consistent with the commit history.

<!-- # tests ------------------------------------------------------------- # -->

## Tests

Changes that affect behavior should include appropriate tests whenever possible.

Before submitting a Pull Request, run the project's available test suite and
verify that existing tests continue to pass.\
If a change cannot reasonably be tested automatically, explain how it was
tested manually in the Pull Request.\
When fixing a bug, adding a regression test is strongly encouraged
when practical.

<!-- # documentation ----------------------------------------------------- # -->

## Documentation

Documentation is an important part of the project.\
If your contribution changes user-facing behavior, APIs, configuration,
installation, commands, or workflows, please update the relevant documentation.

**Documentation contributions are also welcome independently.**

You do not need to write perfect documentation on your first attempt.\
Clear and useful information is more important than perfect wording.

<!-- # review process ---------------------------------------------------- # -->

## Review Process

Pull Requests may be reviewed before they are merged.\
Reviewers may request changes related to:

- Correctness.
- Security.
- Performance.
- Maintainability.
- Testing.
- Documentation.
- Compatibility.
- Project conventions.
- Scope of the contribution.

**Code review is part of collaboration, not a personal judgment.**

Please treat review comments as an opportunity to improve the contribution
and the project.\
Likewise, reviewers should provide feedback that is clear, constructive, and
focused on the code or proposed change.

<!-- # changes requested # ------------------------------------------------- -->

## Responding to Review

If changes are requested, update your branch and push the new commits.\
There is no need to rewrite history unless specifically requested or
required by the project's workflow.

**If you disagree with a review comment, explain your reasoning respectfully.**\
Technical disagreement is welcome when it remains constructive and focused on
finding the best solution for the project.

<!-- # keeping pull requests clean --------------------------------------- # -->

## Keeping a Pull Request Clean

Before requesting a final review, check your changes and make sure the
Pull Request contains only what is necessary.\
Please avoid including:

- Generated files that should not be committed.
- Build artifacts.
- Local configuration files.
- Credentials or secrets.
- Temporary debugging code.
- Unrelated formatting changes.
- Changes to unrelated parts of the project.

A clean Pull Request is easier to review and more likely to be
understood correctly.

<!-- # merge ------------------------------------------------------------- # -->

## Merging

A Pull Request may be merged when:

- The proposed change is understood and considered appropriate.
- Required checks are passing.
- Relevant tests have been added or updated.
- Documentation has been updated when necessary.
- Review feedback has been addressed.
- The contribution follows the project's conventions.

**The final decision to merge a contribution remains with the
project maintainers.**

Not every contribution will necessarily be accepted.\
Sometimes a proposed change may not fit the project's current direction,
architecture, scope, or priorities.\
When possible, maintainers will explain the reasoning behind such decisions.

<!-- # contributor recognition ------------------------------------------- # -->

## Contributor Recognition

**Every contribution is appreciated.**

Contributors may be recognized through Git history, release notes, project
documentation, contributor lists, or other appropriate project channels.\
If you would like your contribution to be attributed to a specific name or
handle, please use that identity consistently in your commits
and Pull Requests.

<!-- # questions --------------------------------------------------------- # -->

## Questions

If you are unsure about how to contribute, what approach to take, or whether
a change would be useful, feel free to start a discussion before investing
significant time in the implementation.

**Asking questions is part of contributing.**\
You do not need to know everything before making your first contribution.

<!-- # final message ----------------------------------------------------- # -->

## Final Note

**There is no contribution that is too small when it helps make the
project better.**

A typo fix, a documentation improvement, a test, a bug report, a performance
improvement, or a new feature can all make a meaningful difference.\
Thank you for taking the time to contribute, improve the project, and help
make software development a better experience for everyone.
