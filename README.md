# 📘 SquadStatsBot Translations
This repository contains language files for the **SquadStats Discord Bot**. These files allow the bot to support multiple languages, making it more accessible and user-friendly around the world.

---
## 📁 Structure

All translation files are stored in the `locales/` folder.

* `en.json`: Is the base file, English (default and reference).
* `fr.json`, `de.json`, etc.: Other language files.

Each file is a JSON object structured by category and string key:

```json
{
  "serverstats": {
    "1": {
      "default": "Server kill Stats",
      "translated": "Statistiques de kill serveur"
    }
  }
}
```

* `default`: The original English text (always from `en.json`)
* `translated`: The translated version in the target language

> ⚠️ Never change `default` fields in translation files. These are automatically synced.

---

## 🌍 Adding a New Language
Want to help translate the bot into your language? Great!

### 🔹 Step 1: Request the Language

Before adding a new language yourself, **please open an issue or discussion** in this repository titled:
**"Request: Add \[Your Language Name]"**

This lets the maintainer:

* Add an official entry for your language
* Generate a proper template file with all required keys
* Ensure consistency with the sync system

### 🔹 Step 2: Translate

Once your language file is created (e.g., `locales/es.json` for Spanish), you can:

* Open it
* Fill in the `"translated"` values
* Leave `"default"` values unchanged

### 🔹 Step 3: Submit a Pull Request

When you're ready, create a PR with:

* Title: `Add Spanish translations` or `Update Turkish translations`
* Description: What you translated or improved

---

## 🔁 Syncing

Whenever the English file (`en.json`) is updated, the translation files will be updated to:

* Adds any new keys
* Ensure `default` values stay in sync
* Remove unused entries (if deleted from `en.json`)

> You don't need to manually manage structure or categories — just translate the `translated` fields.

---

## 🧪 Testing Your Edits

You can use any JSON linter (like [jsonlint.com](https://jsonlint.com)) to verify your files.

Make sure:

* Your file is valid JSON
* Every object has both `default` and `translated` keys

---

## 🙌 Contributing

Everyone is welcome to contribute translations!

### 🛠 Rules

* Do **not** modify the default translation file, `en.json`
* Do **not** change `default` values in translation files
* Use the existing key structure and format

### ✅ Checklist Before PR

* [ ] Only edited `translated` fields
* [ ] File is valid JSON
* [ ] Language file was pre-generated (not manually created)

If you're unsure about something — open an issue and ask!

---

## 📬 Contact

Maintained by [@Tobydeteckel](https://github.com/Tobydeteckel)

If you have any suggestions, improvements, or run into issues, feel free to open a GitHub Issue or contact our discord @ [squadstats.nl/discord](https://squadstats.nl/discord)

---

Thank you for helping make SquadStats better for everyone! 🌍💬
