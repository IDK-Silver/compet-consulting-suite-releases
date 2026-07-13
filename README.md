# Compet Consulting Suite Windows Releases

This public repository contains signed Windows x64 releases for the private `IDK-Silver/compet-consulting-suite` source repository.

## Scope

- Windows x64 only.
- GitHub Releases contain `Setup.exe`, `*-full.nupkg`, and `RELEASES` for Squirrel.Windows auto-update.
- This repository does not contain the private application source, company data, signing certificates, or CI/CD credentials.
- Publicly downloadable installers do not grant access to company data. Application access remains protected by Google OIDC and the server-side account allowlist.

## Release policy

Releases are created by the private source repository through the pinned reusable workflow in `IDK-Silver/ci-workflows`. A release is uploaded as a draft and published only after all required assets and Authenticode signatures pass validation.

Published releases are immutable. Existing tags and assets must not be overwritten; fixes require a new SemVer version.

Do not manually upload, replace, or delete update assets. Support and source changes belong in the private project repository.
