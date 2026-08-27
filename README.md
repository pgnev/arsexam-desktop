# ArsExam Desktop — Legacy Compatibility Repository

Това repository се пази **само за обратна съвместимост** с по-стари ArsExam Desktop инсталации и compatibility URL-и.

> **Не използвайте това repository като текущ download, release или update authority.**

## Текущ официален канал

Официалните ArsExam Windows installers, update packages, Stable/Test manifests, release notes и публични legal/privacy/security notices се публикуват в:

**`pgnev/arsexam-releases`**

Към 27.08.2026 г. текущият официален Stable е **ArsExam 3.2.0**. Test каналът временно е синхронизиран със същата версия и няма активен prerelease.

Текущият application source code не се разпространява от това repository.

## Защо repository-то остава онлайн

По-стари ArsExam клиенти могат все още да използват compatibility URL-и под `pgnev/arsexam-desktop`. Премахването им без контролирана migration логика може да наруши обновяването на стари инсталации.

Затова repository-то може да съдържа само:

- compatibility update metadata;
- минимални compatibility механизми, необходими за стари клиенти;
- copyright/licensing/security notices;
- ясно пренасочване към текущия distribution authority.

То **не трябва да се превръща във втори независим release канал** и не трябва да публикува алтернативни Stable/Test binaries.

## Текуща продуктова линия

ArsExam 3.2.0 включва защитено локално security envelope/SQLCipher-capable SQLite storage, local Recovery Key с encrypted profile-bound vault за нови 3.2+ профили, protected Backup/Restore, Desktop↔Portable Transfer и opt-in crash/error diagnostics.

Това legacy repository:

- не е password-recovery backend;
- не е Backup/Transfer backend;
- не е diagnostics endpoint;
- не съхранява потребителски ArsExam профили, бази или изпитно съдържание.

Няма Supabase recovery service, Request ID или support-issued reset code, свързани с този repository.

## Security boundary

Тук не трябва да се commit-ват application source code, credentials, signing material, private diagnostics, user databases, Recovery Keys, Backup passwords, Transfer codes или examination content.

Compatibility metadata трябва да сочи само към контролирания официален distribution path и не трябва тихо да downgrade-ва клиент към по-стара или непроверена версия.

Security проблеми се докладват частно на **petkoganev@gmail.com**. Вижте `SECURITY.md`.

## Licensing

ArsExam е **proprietary software**. Публичната видимост на това compatibility repository не предоставя MIT, GPL, Apache или друг open-source лиценз върху оригиналния ArsExam софтуер.

Официалните ArsExam binaries се използват съгласно EULA, публикувана с официалната дистрибуция в `pgnev/arsexam-releases`. Third-party компонентите запазват собствените си лицензи и notices.

Вижте `LICENSE.md` и `COPYRIGHT.md`.

## Copyright и support

Copyright © 2026 Petko Ganev. All rights reserved.

Support: **petkoganev@gmail.com**

За текущи releases, инсталатори, manifests, Privacy Policy, EULA и публична продуктова информация използвайте **`pgnev/arsexam-releases`**.
