# Next RP — Localization

<a id="top"></a>

[![English](https://img.shields.io/badge/%F0%9F%87%AC%F0%9F%87%A7-English-2ea44f?style=for-the-badge)](#-english)
[![Русский](https://img.shields.io/badge/%F0%9F%87%B7%F0%9F%87%BA-%D0%A0%D1%83%D1%81%D1%81%D0%BA%D0%B8%D0%B9-1f6feb?style=for-the-badge)](#-русский)
[![Deutsch](https://img.shields.io/badge/%F0%9F%87%A9%F0%9F%87%AA-Deutsch-d73a49?style=for-the-badge)](#-deutsch)
[![Polski](https://img.shields.io/badge/%F0%9F%87%B5%F0%9F%87%B1-Polski-9b59b6?style=for-the-badge)](#-polski)
[![Français](https://img.shields.io/badge/%F0%9F%87%AB%F0%9F%87%B7-Fran%C3%A7ais-0055a4?style=for-the-badge)](#-français)
[![Español](https://img.shields.io/badge/%F0%9F%87%AA%F0%9F%87%B8-Espa%C3%B1ol-e63946?style=for-the-badge)](#-español)
[![Italiano](https://img.shields.io/badge/%F0%9F%87%AE%F0%9F%87%B9-Italiano-009246?style=for-the-badge)](#-italiano)
[![Português](https://img.shields.io/badge/%F0%9F%87%B5%F0%9F%87%B9-Portugu%C3%AAs-046a38?style=for-the-badge)](#-português)
[![Türkçe](https://img.shields.io/badge/%F0%9F%87%B9%F0%9F%87%B7-T%C3%BCrk%C3%A7e-e30a17?style=for-the-badge)](#-türkçe)
[![العربية](https://img.shields.io/badge/%F0%9F%87%B8%F0%9F%87%A6-%D8%A7%D9%84%D8%B9%D8%B1%D8%A8%D9%8A%D8%A9-000000?style=for-the-badge)](#-العربية)
[![中文](https://img.shields.io/badge/%F0%9F%87%A8%F0%9F%87%B3-%E4%B8%AD%E6%96%87-de2910?style=for-the-badge)](#-中文)
[![日本語](https://img.shields.io/badge/%F0%9F%87%AF%F0%9F%87%B5-日本語-bc002d?style=for-the-badge)](#-日本語)
[![한국어](https://img.shields.io/badge/%F0%9F%87%B0%F0%9F%87%B7-한국어-003478?style=for-the-badge)](#-한국어)
[![हिन्दी](https://img.shields.io/badge/%F0%9F%87%AE%F0%9F%87%B3-%E0%A4%B9%E0%A4%BF%E0%A4%A8%E0%A5%8D%E0%A4%A6%E0%A5%80-ff9933?style=for-the-badge)](#-हिन्दी)

> Next RP localization repository. Required languages: **`en`**, **`ru`**, **`de`**, **`pl`**, **`fr`**. Optional languages: `es`, `it`, `pt`, `tr`, `ar`, `zh`, `ja`, `ko`, `hi`. Every PR is auto-validated via `npm test`.

---

# 🇬🇧 English

Hey! First time here? No worries — it’s simpler than it looks.

## Before you start

* All strings live in `.js` files grouped by system folders.
* Every translation entry uses language keys.
* Required languages: `en`, `ru`, `de`, `pl`, `fr`
* Optional languages are welcome.
* Every PR is validated automatically with `npm test`.

## Translation format

```js
loginRecovery: {
    en: 'Login Recovery',
    ru: 'Восстановление логина',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    fr: 'Récupération de connexion',
},
```

## Rules

* Never skip required languages.
* Keep placeholders identical across all languages.
* Do not use `${...}` template literals.
* No unsafe HTML or JavaScript.

[⬆ Back to top](#top)

---

# 🇷🇺 Русский

Привет! Добро пожаловать в систему локализации Next RP.

## Основное

* Все строки находятся в `.js` файлах.
* Обязательные языки: `en`, `ru`, `de`, `pl`, `fr`
* PR автоматически проверяются через `npm test`.

## Формат

```js
loginRecovery: {
    en: 'Login Recovery',
    ru: 'Восстановление логина',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    fr: 'Récupération de connexion',
},
```

[⬆ Наверх](#top)

---

# 🇩🇪 Deutsch

Willkommen beim Next RP Übersetzungsprojekt.

## Wichtig

* Alle Texte liegen in `.js` Dateien.
* Pflichtsprachen: `en`, `ru`, `de`, `pl`, `fr`
* Jeder PR wird automatisch geprüft.

## Format

```js
loginRecovery: {
    en: 'Login Recovery',
    ru: 'Восстановление логина',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    fr: 'Récupération de connexion',
},
```

[⬆ Nach oben](#top)

---

# 🇵🇱 Polski

Witaj w projekcie tłumaczeń Next RP.

## Ważne

* Wszystkie teksty są w plikach `.js`.
* Wymagane języki: `en`, `ru`, `de`, `pl`, `fr`
* Każdy PR przechodzi automatyczne testy.

## Format

```js
loginRecovery: {
    en: 'Login Recovery',
    ru: 'Восстановление логина',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    fr: 'Récupération de connexion',
},
```

[⬆ Do góry](#top)

---

# 🇫🇷 Français

Bienvenue dans le projet de localisation Next RP.

## Important

* Toutes les chaînes sont stockées dans des fichiers `.js`.
* Langues obligatoires : `en`, `ru`, `de`, `pl`, `fr`
* Chaque PR est vérifiée automatiquement.

## Format

```js
loginRecovery: {
    en: 'Login Recovery',
    ru: 'Восстановление логина',
    de: 'Login-Wiederherstellung',
    pl: 'Odzyskiwanie loginu',
    fr: 'Récupération de connexion',
},
```

[⬆ Retour en haut](#top)

---

# 🌍 Additional Languages

## 🇪🇸 Español

Las traducciones opcionales son bienvenidas.

## 🇮🇹 Italiano

Le traduzioni opzionali sono benvenute.

## 🇵🇹 Português

Traduções opcionais são bem-vindas.

## 🇹🇷 Türkçe

İsteğe bağlı çeviriler kabul edilir.

## 🇸🇦 العربية

الترجمات الإضافية مرحب بها.

## 🇨🇳 中文

欢迎提交额外翻译。

## 🇯🇵 日本語

追加翻訳を歓迎します。

## 🇰🇷 한국어

추가 번역 기여를 환영합니다.

## 🇮🇳 हिन्दी

अतिरिक्त अनुवादों का स्वागत है।

---

Thanks for contributing! · Спасибо за вклад! · Danke fürs Mitmachen! · Dzięki za wkład! · Merci pour votre contribution!
