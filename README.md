# Next RP — Localization

<a id="top"></a>

[![English](https://img.shields.io/badge/%F0%9F%87%AC%F0%9F%87%A7-English-2ea44f?style=for-the-badge)](#-english)
[![Deutsch](https://img.shields.io/badge/%F0%9F%87%A9%F0%9F%87%AA-Deutsch-d73a49?style=for-the-badge)](#-deutsch)
[![Polski](https://img.shields.io/badge/%F0%9F%87%B5%F0%9F%87%B1-Polski-9b59b6?style=for-the-badge)](#-polski)
[![Українська](https://img.shields.io/badge/%F0%9F%87%BA%F0%9F%87%A6-Українська-f4d04e?style=for-the-badge)](#-українська)
[![Русский](https://img.shields.io/badge/%F0%9F%87%B7%F0%9F%87%BA-%D0%A0%D1%83%D1%81%D1%81%D0%BA%D0%B8%D0%B9-1f6feb?style=for-the-badge)](#-русский)

> Next RP localization repository. Required languages: **`en`**, **`de`**, **`pl`**, **`ua`**, **`ru`** + optional `fr`, `zh`. Every PR is auto-validated via `npm test`.

---

# 🇬🇧 English

Hey! First time here? No worries — it’s simpler than it looks. Step-by-step below.

## Before you start

- All strings live in `.js` files inside per-system folders (`account/`, `bank/`, `quests/`, etc.).
- Each string is an object with language keys.
- **All 5 languages (`en`, `de`, `pl`, `ua`, `ru`) are required.**
- Every PR is checked by `npm test` — it validates syntax, placeholders, and unsafe code. Red CI = no merge.

## Steps

1. **Fork** this repo (`Fork` button at the top right on GitHub).
2. **Clone your fork** locally:
   ```sh
   git clone https://github.com/<your-username>/next-rp-localization.git
   cd next-rp-localization
   ```

3. **Create a branch** (one branch = one PR):
   ```sh
   git checkout -b fix/account-login-en
   ```

4. **Find the file.**
   Files are grouped by system:
   - login → `account/`
   - bank → `bank/`
   - quests → `quests/`

5. **Edit or add the key.** Format below.

6. **Validate locally** (requires Node.js 20+):
   ```sh
   npm test
   ```

   Green? Move on.  
   Red? Read the output — it points to the exact file and line.

7. **Commit & push:**
   ```sh
   git add .
   git commit -m "account: fix english translation for loginRecovery"
   git push origin fix/account-login-en
   ```

8. **Open a Pull Request** to the `master` branch of the upstream repo. Describe what you changed and why.

## Translation format

```js
loginRecovery: {
    en: 'Login Recovery',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    ua: 'Відновлення логіну',
    ru: 'Восстановление логина',
},
```

## Rules

- Never skip any of the 5 base languages.
- Placeholders like `{{name}}`, `{{amount}}` must match across all languages.
- If `en` contains `{{count}}`, then every other language must contain it too.
- Don’t use `${...}` template literals — plain `'...'` or `"..."` only.
- No `<script>`, `onclick=`, or `javascript:` — the validator will reject it.

## Pre-PR checklist

- [ ] All 5 languages filled (`en`, `de`, `pl`, `ua`, `ru`)
- [ ] Placeholders identical across languages
- [ ] Translation is human, not raw Google Translate
- [ ] `npm test` passes locally
- [ ] Commit message follows `<area>: <what you did>`

[⬆ Back to top](#top)

---

# 🇩🇪 Deutsch

Hi! Zum ersten Mal hier? Keine Sorge — es ist einfacher, als es aussieht. Schritt für Schritt unten.

## Bevor du loslegst

- Alle Strings befinden sich in `.js`-Dateien innerhalb der Systemordner (`account/`, `bank/`, `quests/` usw.).
- Jeder String ist ein Objekt mit Sprachschlüsseln.
- **Alle 5 Sprachen (`en`, `de`, `pl`, `ua`, `ru`) sind Pflicht.**
- Jeder PR wird durch `npm test` geprüft — Syntax, Platzhalter und unsicherer Code werden validiert. Rotes CI = kein Merge.

## Schritte

1. **Erstelle einen Fork** dieses Repositories.
2. **Klone deinen Fork** lokal:
   ```sh
   git clone https://github.com/<dein-name>/next-rp-localization.git
   cd next-rp-localization
   ```

3. **Erstelle einen Branch** (ein Branch = ein PR):
   ```sh
   git checkout -b fix/account-login-de
   ```

4. **Finde die richtige Datei.**
   Dateien sind nach Systemen sortiert:
   - Login → `account/`
   - Bank → `bank/`
   - Quests → `quests/`

5. **Bearbeite oder ergänze den Schlüssel.**

6. **Lokal prüfen** (Node.js 20+ erforderlich):
   ```sh
   npm test
   ```

   Grün? Weiter.  
   Rot? Lies die Ausgabe — dort stehen Datei und Zeile.

7. **Committen & Pushen:**
   ```sh
   git add .
   git commit -m "account: fix german translation for loginRecovery"
   git push origin fix/account-login-de
   ```

8. **Öffne einen Pull Request** gegen den `master`-Branch des Hauptrepositories. Beschreibe, was du geändert hast und warum.

## Übersetzungsformat

```js
loginRecovery: {
    en: 'Login Recovery',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    ua: 'Відновлення логіну',
    ru: 'Восстановление логина',
},
```

## Regeln

- Keine der 5 Basissprachen auslassen.
- Platzhalter wie `{{name}}` oder `{{amount}}` müssen überall identisch sein.
- Wenn `en` ein `{{count}}` enthält, müssen alle anderen Sprachen es ebenfalls enthalten.
- Keine `${...}`-Template-Strings verwenden.
- Kein `<script>`, `onclick=` oder `javascript:`.

## Pre-PR-Checkliste

- [ ] Alle 5 Sprachen ausgefüllt (`en`, `de`, `pl`, `ua`, `ru`)
- [ ] Platzhalter überall identisch
- [ ] Übersetzung von Hand geschrieben
- [ ] `npm test` lokal erfolgreich
- [ ] Commit-Message im Format `<bereich>: <änderung>`

[⬆ Nach oben](#top)

---

# 🇵🇱 Polski

Cześć! Pierwszy raz tutaj? Spokojnie — to prostsze, niż wygląda. Instrukcja krok po kroku poniżej.

## Zanim zaczniesz

- Wszystkie teksty znajdują się w plikach `.js` w folderach systemów (`account/`, `bank/`, `quests/` itd.).
- Każdy wpis jest obiektem z kluczami językowymi.
- **Wszystkie 5 języków (`en`, `de`, `pl`, `ua`, `ru`) jest wymagane.**
- Każdy PR jest sprawdzany przez `npm test` — sprawdzana jest składnia, placeholdery i niebezpieczny kod.

## Krok po kroku

1. **Zrób fork** repozytorium.
2. **Sklonuj swojego forka** lokalnie:
   ```sh
   git clone https://github.com/<twój-login>/next-rp-localization.git
   cd next-rp-localization
   ```

3. **Utwórz branch** (jeden branch = jeden PR):
   ```sh
   git checkout -b fix/account-login-pl
   ```

4. **Znajdź odpowiedni plik.**
   - login → `account/`
   - bank → `bank/`
   - questy → `quests/`

5. **Dodaj lub edytuj klucz.**

6. **Uruchom testy lokalnie** (Node.js 20+):
   ```sh
   npm test
   ```

   Zielone? Lecimy dalej.  
   Czerwone? Output pokaże dokładny plik i linię.

7. **Commit i push:**
   ```sh
   git add .
   git commit -m "account: fix polish translation for loginRecovery"
   git push origin fix/account-login-pl
   ```

8. **Otwórz Pull Request** do brancha `master` głównego repozytorium. Opisz, co zmieniłeś i dlaczego.

## Format tłumaczenia

```js
loginRecovery: {
    en: 'Login Recovery',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    ua: 'Відновлення логіну',
    ru: 'Восстановление логина',
},
```

## Zasady

- Nie pomijaj żadnego z 5 podstawowych języków.
- Placeholdery muszą być identyczne we wszystkich językach.
- Jeśli `en` zawiera `{{count}}`, pozostałe języki również muszą go zawierać.
- Nie używaj `${...}`.
- Bez `<script>`, `onclick=` i `javascript:`.

## Checklista przed PR

- [ ] Wszystkie 5 języków uzupełnione (`en`, `de`, `pl`, `ua`, `ru`)
- [ ] Placeholdery identyczne
- [ ] Tłumaczenie napisane przez człowieka
- [ ] `npm test` przechodzi poprawnie
- [ ] Commit message ma poprawny format

[⬆ Do góry](#top)

---

# 🇺🇦 Українська

Привіт! Якщо ти тут уперше — не хвилюйся, усе простіше, ніж здається. Покрокова інструкція нижче.

## Що потрібно знати

- Усі рядки знаходяться у `.js`-файлах у папках систем (`account/`, `bank/`, `quests/` тощо).
- Кожен рядок — це обʼєкт із мовними ключами.
- **Усі 5 мов (`en`, `de`, `pl`, `ua`, `ru`) є обовʼязковими.**
- Кожен PR перевіряється через `npm test` — перевіряються синтаксис, плейсхолдери та небезпечний код.

## Покроково

1. **Зроби fork** репозиторію.
2. **Склонуй fork локально:**
   ```sh
   git clone https://github.com/<твій-нік>/next-rp-localization.git
   cd next-rp-localization
   ```

3. **Створи branch** (один branch = один PR):
   ```sh
   git checkout -b fix/account-login-ua
   ```

4. **Знайди потрібний файл.**
   - логін → `account/`
   - банк → `bank/`
   - квести → `quests/`

5. **Відредагуй або додай ключ.**

6. **Перевір локально** (Node.js 20+):
   ```sh
   npm test
   ```

   Зелене? Рухаймося далі.  
   Червоне? У виводі буде вказано файл і рядок.

7. **Зроби commit і push:**
   ```sh
   git add .
   git commit -m "account: fix ukrainian translation for loginRecovery"
   git push origin fix/account-login-ua
   ```

8. **Відкрий Pull Request** у `master` основного репозиторію. Опиши, що змінив і навіщо.

## Формат перекладу

```js
loginRecovery: {
    en: 'Login Recovery',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    ua: 'Відновлення логіну',
    ru: 'Восстановление логина',
},
```

## Правила

- Не пропускай жодну з 5 мов.
- Плейсхолдери мають бути однаковими в усіх мовах.
- Якщо `en` містить `{{count}}`, інші мови також повинні його містити.
- Не використовуй `${...}`.
- Без `<script>`, `onclick=` і `javascript:`.

## Чек-лист перед PR

- [ ] Усі 5 мов заповнені (`en`, `de`, `pl`, `ua`, `ru`)
- [ ] Плейсхолдери однакові
- [ ] Переклад написаний людиною
- [ ] `npm test` проходить успішно
- [ ] Commit message у правильному форматі

[⬆ Нагору](#top)

---

# 🇷🇺 Русский

Привет! Если ты здесь впервые — не переживай, всё проще, чем кажется. Пошаговая инструкция ниже.

## Что нужно знать

- Все строки находятся в `.js`-файлах по папкам (`account/`, `bank/`, `quests/` и т.д.).
- Каждая строка — объект с языковыми ключами.
- **Все 5 языков (`en`, `de`, `pl`, `ua`, `ru`) обязательны.**
- Каждый PR проверяется через `npm test` — проверяются синтаксис, плейсхолдеры и небезопасный код.

## Пошагово

1. **Сделай fork** репозитория.
2. **Склонируй fork локально:**
   ```sh
   git clone https://github.com/<твой-ник>/next-rp-localization.git
   cd next-rp-localization
   ```

3. **Создай branch** (одна ветка = один PR):
   ```sh
   git checkout -b fix/account-login-ru
   ```

4. **Найди нужный файл.**
   - логин → `account/`
   - банк → `bank/`
   - квесты → `quests/`

5. **Отредактируй или добавь ключ.**

6. **Проверь локально** (Node.js 20+):
   ```sh
   npm test
   ```

   Зелёный результат? Продолжай.  
   Красный? В выводе будет указан файл и строка.

7. **Сделай commit и push:**
   ```sh
   git add .
   git commit -m "account: fix russian translation for loginRecovery"
   git push origin fix/account-login-ru
   ```

8. **Открой Pull Request** в `master` основного репозитория. Опиши, что изменил и зачем.

## Формат строки

```js
loginRecovery: {
    en: 'Login Recovery',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    ua: 'Відновлення логіну',
    ru: 'Восстановление логина',
},
```

## Правила

- Не пропускай ни один из 5 языков.
- Плейсхолдеры должны совпадать во всех языках.
- Если в `en` есть `{{count}}`, он должен быть и во всех остальных языках.
- Не используй `${...}`.
- Без `<script>`, `onclick=` и `javascript:`.

## Чек-лист перед PR

- [ ] Все 5 языков заполнены (`en`, `de`, `pl`, `ua`, `ru`)
- [ ] Плейсхолдеры одинаковые
- [ ] Перевод написан человеком
- [ ] `npm test` проходит успешно
- [ ] Commit message в правильном формате

[⬆ Наверх](#top)

---

Thanks for contributing! · Дякуємо за внесок! · Danke fürs Mitmachen! · Dzięki za wkład! · Спасибо за вклад!
