# Contributing to CAPITA

CAPITA is a SAS microsimulation model of the Australian tax-and-transfer system. Read the [README](README.md) and [license](LICENSE) before contributing, including the separate software and microdata access requirements.

## Before you start

Search existing issues and pull requests before starting, and discuss substantial changes or new dependencies in an issue. Use an issue template when one is offered. For a bug, include the affected commit or version, environment, a minimal reproduction, and expected versus observed behavior; remove sensitive information from logs and screenshots.

## Development and validation

Preserve the directory structure described in [DefineCapitaDirectory.sas](DefineCapitaDirectory.sas). Review [RunCapita.sas](RunCapita.sas) for the year, quarter, duration, policy switches, and module sequence relevant to your change; do not substitute personal paths or restricted input data into committed examples.

Use an authorized SAS environment and licensed inputs for execution. Document the policy period, parameter sources, run settings, and affected modules. For a calculation change, provide a small synthetic household example with independently calculated expected results, including boundary cases, and compare affected outputs. Record checks that depend on unavailable microdata separately from completed checks. Maintain the existing variable and output contracts, or explain any intentional compatibility change.

## Pull requests

Work on a focused branch from the current default branch. Open a pull request explaining the problem, the resulting behavior, and any compatibility or data-format changes. Link the relevant issue and complete any existing PR template.

Add focused regression coverage for changed behavior and update affected examples or documentation. Describe the checks actually run, their results, and any checks you could not run. For documentation-only changes, verify links, examples, and rendered formatting. Use the repository's existing checks and review/merge process; preserve required checks and resolve actionable feedback without weakening the checks.

## Security and sensitive information

Follow the [account security policy](https://github.com/edithatogo/.github/blob/main/SECURITY.md). Report vulnerabilities privately through the repository's **Report a vulnerability** option if available; otherwise request a private reporting contact without posting exploit details. Never include credentials, personal information, restricted datasets, or confidential records in issues, commits, fixtures, or diagnostic output.

## Licensing and conduct

Be respectful and constructive, and follow the [account code of conduct](https://github.com/edithatogo/.github/blob/main/CODE_OF_CONDUCT.md). Preserve attribution and third-party notices. Contribute only material you are entitled to share; resolve unclear permissions before adding third-party content. This guide does not change licensing terms or introduce a CLA or DCO requirement.

## References

- [GitHub contribution guideline conventions](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors)
- [OpenSSF contribution and quality criteria](https://www.bestpractices.dev/en/criteria)
