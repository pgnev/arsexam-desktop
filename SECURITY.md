# ArsExam Desktop — Retired Repository Security Notice

This repository is **retired** and is not part of the current ArsExam source, release or update architecture.

## Report privately

Report suspected ArsExam vulnerabilities privately to **petkoganev@gmail.com** with subject `ArsExam security report`.

Do not publish exploitable details, credentials, Recovery Keys, Backup passwords, Transfer credentials, private diagnostics, databases or examination content in public issues.

## Repository security boundary

This repository must not contain:

- current ArsExam application source code;
- current Stable/Test update manifests;
- user profiles or databases;
- Recovery Keys, Backup passwords or Transfer credentials;
- signing/private keys or GitHub write credentials;
- private diagnostic events;
- confidential examination content.

## Current authority

The sole official public distribution/update authority is **`pgnev/arsexam-releases`**.

The private canonical source/development repository is **`pgnev/arsexam-source`**.

The ArsExam 3.5.1 candidate has removed runtime update fallback to `pgnev/arsexam-desktop`; this repository is therefore no longer an active compatibility dependency.

Current public Stable: **3.5.0**.  
Current development / acceptance candidate: **3.5.1 — NOT RELEASED**.

## Historical content

Any legacy manifests, compatibility metadata, tags or release objects remaining here are historical artifacts only. They must not be treated as current download/update authority and must not be modified to create a second distribution channel.

## No recovery backend here

This repository is not a password-recovery, Backup, Transfer or diagnostics backend. ArsExam uses local Recovery Key recovery and does not rely on a server-side master password, support-issued reset code or this repository for recovery.
