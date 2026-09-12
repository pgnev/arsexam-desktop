# ArsExam Desktop — Retired Repository Security Notice

This repository is **retired** and is not part of the current ArsExam source, release or update architecture.

## Report privately

Report suspected ArsExam vulnerabilities privately to **petkoganev@gmail.com** with subject `ArsExam security report`.

Do not publish exploitable details, credentials, Recovery Keys, Backup passwords, Transfer credentials, private diagnostics, databases or examination content in public issues.

## Repository security boundary

This repository must not contain:

- current ArsExam application source code;
- current Stable/Test update manifests for supported current clients;
- user profiles or databases;
- Recovery Keys, Backup passwords or Transfer credentials;
- signing/private keys or GitHub write credentials;
- private diagnostic events;
- confidential examination content.

## Current authority

The sole official public distribution/update authority is **`pgnev/arsexam-releases`**.

The private canonical source/development repository is **`pgnev/arsexam-source`**.

This retired repository deliberately does **not** hard-code a current Stable or development version. Current public Stable identity is determined by:

- `pgnev/arsexam-releases/update/stable-manifest.json`;
- the latest non-draft, non-prerelease public release in `pgnev/arsexam-releases`.

Current supported ArsExam versions use the official feeds in `pgnev/arsexam-releases`. This repository is retained only for legacy compatibility: early ArsExam Desktop clients, including the historical 3.0.1 line, may still contain a hard-coded update URL under `pgnev/arsexam-desktop`.

Therefore this repository must remain frozen and public until the canonical release policy explicitly retires that legacy compatibility path or a validated replacement bridge is in place. It must not be treated as a second current distribution authority.

## Historical content

Any legacy manifests, compatibility metadata, tags or release objects remaining here are historical artifacts only. They must not be treated as current download/update authority and must not be modified to create a second distribution channel.

The legacy `update/test-manifest.json` and historical release/tag metadata remain compatibility/history evidence; they do not define the current Test or Stable channel for supported clients.

## No recovery backend here

This repository is not a password-recovery, Backup, Transfer or diagnostics backend. ArsExam uses local Recovery Key recovery and does not rely on a server-side master password, support-issued reset code or this repository for recovery.
