# ArsExam Desktop — Retired Legacy Repository

Това repository е **retired** и повече не е част от поддържаната ArsExam update/distribution architecture.

> **Не използвайте това repository за download, release, update manifest или текуща продуктова документация.**

## Официален канал

Единственият официален публичен канал за ArsExam Windows installers, update packages, Stable/Test manifests, release notes и публични legal/privacy/security notices е:

**`pgnev/arsexam-releases`**

Каноничният private source/development repository е:

**`pgnev/arsexam-source`**

Текущият public Stable е **ArsExam 3.5.0**. **ArsExam 3.5.1** е development / acceptance candidate и **НЕ Е ПУБЛИКУВАН**.

## Статус на това repository

`pgnev/arsexam-desktop` е използвано исторически като compatibility bridge за ранни ArsExam Desktop update URL-и.

От 3.5.1 candidate:

- runtime fallback-ът към `pgnev/arsexam-desktop` е премахнат от updater-а;
- Stable и Test manifest-ите се четат само от `pgnev/arsexam-releases`;
- public release publisher-ът използва само `pgnev/arsexam-releases`;
- exact-head Windows Release #949 е SUCCESS;
- exact-head Update Upgrade Matrix #419 е SUCCESS;
- няма активна поддържана runtime/workflow зависимост към това repository.

Следователно това repository **може да бъде архивирано** и не трябва да се поддържа като compatibility channel. Окончателното му изтриване е repository housekeeping решение и не е prerequisite за нормалната работа на ArsExam 3.5.1 architecture.

## Исторически `v3.0.2`

Видимият `v3.0.2` release/tag е **исторически compatibility artifact**. Той:

- не е текущ ArsExam Stable release;
- не е официален download;
- не е независим update channel;
- не е authority за текущи manifests или binaries.

За актуални releases използвайте единствено `pgnev/arsexam-releases`.

## Security boundary

Това retired repository не трябва да съдържа:

- текущ ArsExam application source code;
- user profiles или databases;
- Recovery Keys, Backup passwords или Transfer credentials;
- signing/private keys или GitHub write credentials;
- private diagnostic events;
- confidential examination content.

Security проблеми се докладват частно на **petkoganev@gmail.com**. Вижте `SECURITY.md`.

## Licensing

ArsExam е **proprietary software**. Публичната видимост на това historical repository не предоставя open-source лиценз върху оригиналния ArsExam софтуер.

Официалните binaries се използват съгласно EULA и notices, публикувани с официалната дистрибуция в `pgnev/arsexam-releases`.

Вижте `LICENSE.md` и `COPYRIGHT.md`.

## Copyright и support

Copyright © 2026 Petko Ganev. All rights reserved.

Support: **petkoganev@gmail.com**

За текущи releases, installers, manifests, Privacy Policy, EULA и публична продуктова информация използвайте **`pgnev/arsexam-releases`**.
