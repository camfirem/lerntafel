# Security Policy

## Reporting a vulnerability

If you find a security issue in Lerntafel (the installer, the application itself, or its bundled components), please report it privately instead of opening a public issue:

- Preferred: open a [GitHub Security Advisory](../../security/advisories/new) for this repository (private, only visible to the maintainer until resolved).
- Alternative: [open a regular issue](../../issues/new/choose) marked `security` with as little detail as possible in the title, and wait to be contacted before posting specifics.

Please include, where possible:
- A description of the issue and its impact.
- Steps to reproduce, or a minimal example.
- The Lerntafel version and Windows version you tested on.

## What to expect

This is a solo-developer beta project — there is no dedicated security team and no SLA. I aim to acknowledge reports within a few days and to fix confirmed issues in the next release. Please give a reasonable amount of time to fix an issue before any public disclosure.

## Scope

In scope: the Lerntafel installer and application (`Lerntafel-Setup-*.exe`, `Lerntafel.exe`) as distributed through this repository's [Releases](../../releases) page.

Out of scope: third-party services you connect Lerntafel to (Anthropic, OpenAI, Ollama, etc.) — report those directly to the respective provider. See [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) for bundled components and their own upstream projects.
