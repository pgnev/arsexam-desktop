# ArsExam Desktop — Legacy Compatibility Repository

This repository is retained **only for backward compatibility** with older ArsExam Desktop installations released before public binary/update distribution moved to the dedicated release repository.

> **Do not use this repository as the current download or update authority.**

## Current official distribution

Official ArsExam Windows installers, update packages, Stable/Test manifests and public release notices are published in:

**`pgnev/arsexam-releases`**

The current application source code is not distributed from this repository.

## Why this repository remains online

Older ArsExam clients may still contact URLs under `pgnev/arsexam-desktop`. Removing or repurposing those endpoints could break update compatibility for installations that have not yet migrated to the current release infrastructure.

Accordingly, this repository may contain only:

- compatibility update metadata;
- narrowly scoped compatibility workflows;
- minimal public copyright/licensing information.

It must not become a second independent release channel.

## Security boundary

No application source code, credentials, signing material, private diagnostics, user databases or examination content should be committed here.

Compatibility metadata must point only to the controlled official distribution path and must not silently downgrade a client to an older or unverified package.

## Licensing

ArsExam is **proprietary software**. This public compatibility repository does not place ArsExam under an open-source license.

Official ArsExam binaries are governed by the End User License Agreement (EULA) distributed with the corresponding release. Third-party components retain their own licenses and notices.

## Copyright and support

Copyright © 2026 Petko Ganev. All rights reserved.

Support: **petkoganev@gmail.com**

For current releases and public product information, use `pgnev/arsexam-releases`.
