# Damn Vulnerable Exposed Secrets

Various dummy secrets in various formats for security tools testing. 



| Name                                                                      | Description                                                                    | Git Support   | Language   | License    |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------------ | ------------- | ---------- | ---------- |
| [**TruffleHog**](https://github.com/trufflesecurity/trufflehog)           | Find secrets and credentials in repos, files and API. Support JSON/regex/diff. | ✅             | Python     | AGPL-3.0   |
| [**Gitleaks**](https://github.com/gitleaks/gitleaks)                      | Fast and configurable scanner for Git-repos. IDE and CI/CD ready.              | ✅             | Go         | MIT        |
| [**detect-secrets**](https://github.com/Yelp/detect-secrets)              | Plugin-based secret scanner by Yelp. pre-commit and baseline support.          | ⚠️ (diff only) | Python     | Apache-2.0 |
| [**GitGuardian CLI (ggshield)**](https://github.com/GitGuardian/ggshield) | CLI-scanner, find secrets, leaks in repos and CI/CD.                           | ✅             | Python     | MIT        |
| [**Secretlint**](https://github.com/secretlint/secretlint)                | Pluggable linting tool for `.env`, JSON, YAML.                                 | ❌             | TypeScript | MIT        |
| [**Talisman**](https://github.com/thoughtworks/talisman)                  | Git pre-commit hook for blocking leaked tokens/keys.                           | ✅             | Go         | Apache-2.0 |
| [**shhgit**](https://github.com/eth0izzle/shhgit)                         | Realtime GitHub monitoring.                                                    | ❌             | Go         | MIT        |



> [!WARNING]  
> OSS Version of Trufflehog have scan source limitations. See [documentation](https://docs.trufflesecurity.com/scan-data-for-secrets).


Recomendations:
- CI/CD integrations: Gitleaks, ggshield, detect-secrets, trufflehog.
- Pre-commit hooks: detect-secrets, talisman, gitleaks.
- Scan files without git: detect-secrets, secretlint, ggshield.