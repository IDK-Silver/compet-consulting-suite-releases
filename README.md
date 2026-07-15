# Compet Consulting Suite Windows Releases

This public repository hosts Windows x64 releases for the private `IDK-Silver/compet-consulting-suite` source repository.

## Download

Latest installer:

<https://github.com/IDK-Silver/compet-consulting-suite-releases/releases/latest/download/CompetConsultingSuiteSetup.exe>

Releases are currently **not code-signed**. Windows SmartScreen will warn on first run; choose "More info" → "Run anyway". Authenticode signing is planned once a company certificate is available.

## Scope

- Windows x64 only.
- Each GitHub Release contains `CompetConsultingSuiteSetup.exe`, `*-full.nupkg`, and `RELEASES` for Squirrel.Windows auto-update via `update.electronjs.org`.
- This repository does not contain the private application source, company data, signing certificates, or CI/CD credentials.
- Publicly downloadable installers do not grant access to company data. Application access remains protected by Google OIDC and the server-side account allowlist.

## Release policy

Releases are created by GitHub Actions in the private source repository (`desktop-v*` tags trigger `electron-forge publish`).

Published releases are immutable. Existing tags and assets must not be overwritten; fixes require a new SemVer version.

Do not manually upload, replace, or delete update assets. Support and source changes belong in the private project repository.
