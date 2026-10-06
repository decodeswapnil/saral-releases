# Saral installers

[Download Saral for Mac and Windows](https://updates.saralai.xyz/downloads/)

This public repository contains verified installers, checksums, release notes, and native build automation. Development source stays private in a separate repository. No provider credentials or user data are published.

The workflow polls private numeric version tags every 15 minutes. For an immediate build, run **Build and publish Saral** and enter the version tag. A read-only source deploy key and the persistent Mac signing identity are protected Actions secrets. Native tests and package checks must pass on Apple Silicon, Intel Mac, and Windows x64 before publishing. Only installers and release metadata are uploaded.

Cloudflare receives an authenticated release webhook and updates the in-app discovery manifest. Downloads begin only when the user chooses them. Free community Mac updates require replacing Saral in Applications; Windows uses Setup.exe. No Python or Node.js installation is needed.

Community releases do not carry paid Apple Developer ID/notarization or Windows signing credentials. First-install Gatekeeper or SmartScreen warnings remain possible. Never disable operating-system protections to install or update Saral.
