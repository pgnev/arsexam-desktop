# ArsExam Desktop — Retired Legacy Compatibility Repository

Това repository е **retired** и не е част от текущата ArsExam development/distribution architecture.

> **Не използвайте това repository като текущ download, release, update authority или продуктова документация.**

## Официален канал

Единственият официален публичен канал за ArsExam Windows installers, update packages, Stable/Test manifests, release notes и публични legal/privacy/security notices е:

**`pgnev/arsexam-releases`**

Каноничният private source/development repository е:

**`pgnev/arsexam-source`**

Текущата Stable версия **не се дублира статично в това legacy repository**. Authoritative current Stable identity се определя от:

- `pgnev/arsexam-releases/update/stable-manifest.json`;
- latest public release в `pgnev/arsexam-releases`.

Това предотвратява остарели „current version“ твърдения тук при бъдещи release-и.

## Защо repository-то все още не трябва да се изтрива

`pgnev/arsexam-desktop` е използвано исторически от ранни ArsExam Desktop updater-и. По-конкретно ArsExam **3.0.1** съдържа hard-coded Stable URL към:

`https://github.com/pgnev/arsexam-desktop/releases/latest/download/update-manifest.json`

Следователно изтриването на repository-то би прекъснало този исторически update endpoint за инсталации, които още разчитат на него.

Текущите ArsExam версии четат официалните Stable/Test feeds от `pgnev/arsexam-releases`, а от 3.5.1 насам няма активен runtime fallback към това repository. Въпреки това compatibility endpoint-ът за по-старите клиенти трябва първо да бъде изведен от support или заменен с доказан migration bridge.

**Статус:** repository-то е оперативно неактивно и трябва да остане замразено. **Не го изтривайте и не го правете private**, докато canonical release policy изрично не обяви legacy 3.0.x update path за неподдържан или не бъде валидиран replacement bridge.

## Исторически `v3.0.2`

Видимият `v3.0.2` release/tag е исторически compatibility artifact. Той:

- не е текущ ArsExam Stable release;
- не е официален download;
- не е независим update channel;
- не е authority за текущи manifests или binaries.

Compatibility metadata не трябва да се използва за нови инсталации. За актуални releases използвайте единствено `pgnev/arsexam-releases`.

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
