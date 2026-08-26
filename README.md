# ArsExam Desktop — Legacy Compatibility Repository

Това repository се пази **само за обратна съвместимост** с по-стари ArsExam Desktop инсталации, публикувани преди официалната binary/update дистрибуция да бъде преместена в отделния release repository.

> **Не използвайте това repository като текущ download или update authority.**

## Текуща официална дистрибуция

Официалните ArsExam Windows installers, update packages, Stable/Test manifests и публични release notices се публикуват в:

**`pgnev/arsexam-releases`**

Към момента на тази актуализация публикуваният Stable е **3.1.0**, а **3.1.1** е финален Stable candidate в private validation. След официалната му публикация авторитетният статус винаги е този в `pgnev/arsexam-releases` и неговия Stable manifest.

ArsExam 3.1.1 поддържа clean install и **не изисква предварително инсталиран 3.1.0**. Пълният Setup за 3.1.0 → 3.1.1 е upgrade-path изискване заради Launcher/deployment промени, а не prerequisite за нова инсталация.

Текущият application source code не се разпространява от това repository.

## Защо repository-то остава онлайн

По-стари ArsExam клиенти могат все още да използват compatibility URL-и под `pgnev/arsexam-desktop`. Премахването или пренасочването им без контролирана migration логика може да наруши обновяването на стари инсталации.

Затова repository-то може да съдържа само:

- compatibility update metadata;
- минимални compatibility механизми, когато са необходими за стар клиент;
- публична информация за copyright/licensing и пренасочване към текущия distribution authority.

То не трябва да се превръща във втори независим release канал.

## Текуща продуктова архитектура

Новата функционалност, включително 3.1.1 local Recovery Key, encrypted SQLite/security envelope, protected Backup/Restore, Desktop↔Portable Transfer и opt-in crash/error diagnostics, се разработва и валидира в private canonical source repository и се публикува само чрез `pgnev/arsexam-releases`.

Това legacy repository не е backend за password recovery, Backup, Transfer или диагностика и не съхранява потребителски ArsExam данни.

## Security boundary

Тук не трябва да се commit-ват application source code, credentials, signing material, private diagnostics, user databases или examination content.

Compatibility metadata трябва да сочи само към контролирания официален distribution path и не трябва тихо да downgrade-ва клиент към по-стара или непроверена версия.

## Licensing

ArsExam е **proprietary software**. Това публично compatibility repository не поставя ArsExam под open-source лиценз.

Официалните ArsExam binaries се използват съгласно End User License Agreement (EULA), предоставено със съответния release. Third-party компонентите запазват собствените си лицензи и notices.

## Copyright и support

Copyright © 2026 Petko Ganev. All rights reserved.

Support: **petkoganev@gmail.com**

За текущи releases, инсталатори, manifests и публична продуктова информация използвайте **`pgnev/arsexam-releases`**.
