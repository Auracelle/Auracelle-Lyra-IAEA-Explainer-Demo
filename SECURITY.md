# Security Policy

## Scope

This policy covers the **Auracelle Lyra — IAEA Explainer** in this repository: the single file `index.html` and the GitHub Pages site built from it.

The full Lyra simulation is distributed separately, through secure sign-in, and is outside the scope of this repository.

## Security design

The Explainer is designed to have as little attack surface as possible:

- **Self-contained.** One static HTML file with inline styles and scripts. No third-party libraries, fonts, images or content delivery networks.
- **No network requests.** A Content Security Policy (`default-src 'none'`) blocks all outside connections. The only links are `mailto:` contact addresses, which open only when clicked.
- **No data handling.** No forms, inputs, uploads, cookies, local storage, analytics or tracking. The page collects, stores and transmits nothing.
- **No secrets.** The file contains no passwords, API keys, tokens or credentials.
- **No AI connection.** The Explainer does not call any AI service. Red Team examples are fixed text.
- **Local narration.** Audio uses the browser's built-in speech voice on the viewer's own device.

## Supported versions

| Version | Supported |
|---|---|
| Latest version on the `main` branch | Yes |
| Earlier versions | No |

Fixes are made to the latest version only. Viewers should always use the published GitHub Pages site or the latest `index.html` from `main`.

## Reporting a vulnerability

Please report security concerns **privately**. Do not open a public GitHub issue for a suspected vulnerability.

Email: **[EvansAGrace@gmail.com](mailto:EvansAGrace@gmail.com)**, copying [access@auracelle.ai](mailto:access@auracelle.ai)
Subject line: `Security — Lyra IAEA Explainer`

Please include:

- a description of the issue and why it matters
- the steps to reproduce it, including browser and device
- the version or commit you tested, if known
- any suggested fix

## What to expect

- **Acknowledgement** within 5 business days.
- **Initial assessment** within 10 business days, including whether we can reproduce the issue.
- **A fix or mitigation** as soon as practical, prioritised by severity.
- **Credit** in the release notes if you would like it, once the fix is published.

We ask that you give us reasonable time to address an issue before disclosing it publicly, and that you avoid accessing data that is not yours, degrading the service, or using social engineering.

## Out of scope

- The behaviour of browsers, operating systems or their built-in speech voices
- GitHub and GitHub Pages infrastructure (report these to GitHub)
- The full Lyra simulation, which is covered by its own access terms
- Reports that require physical access to a viewer's device

## Integrity of the published file

The Explainer should be obtained only from this repository or its GitHub Pages site. If you receive a copy from another source, please compare it with the version on `main`, or contact us to confirm it is authentic.
