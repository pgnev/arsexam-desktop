# ArsExam Desktop Legacy Security Notice

This repository is a **legacy compatibility repository**, not the current source or distribution authority.

## Report privately

Report suspected ArsExam vulnerabilities or unsafe compatibility metadata privately to **petkoganev@gmail.com** with subject `ArsExam security report`.

Do not publish exploitable details, credentials, Recovery Keys, Backup passwords, Transfer codes, private diagnostics, databases or examination content in public issues.

## Repository security boundary

This repository must not contain:

- current ArsExam application source code;
- user profiles or databases;
- Recovery Keys, Backup passwords or Transfer codes;
- signing/private keys or GitHub write credentials;
- private diagnostic events;
- confidential examination content.

Compatibility metadata must point only to the controlled official distribution path and must not silently downgrade clients to obsolete or unverified binaries.

## Current authority

The official public distribution/update authority is **`pgnev/arsexam-releases`**. Current security, privacy, EULA and support notices are maintained there.

The private canonical source repository is `pgnev/arsexam-source`.

## No recovery backend here

This repository is not a password-recovery service. ArsExam 3.2.0 uses local Recovery Key recovery and does not rely on Supabase recovery e-mail, Request ID or support-issued reset codes.
