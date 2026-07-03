# 🌍 World Holidays Data

[![GitHub Stars](https://img.shields.io/github/stars/eramitgupta/world-holidays-data?style=social)](https://github.com/eramitgupta/world-holidays-data/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/eramitgupta/world-holidays-data?style=social)](https://github.com/eramitgupta/world-holidays-data/network/members)
[![GitHub Issues](https://img.shields.io/github/issues/eramitgupta/world-holidays-data)](https://github.com/eramitgupta/world-holidays-data/issues)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> ⭐ If this project helps you, please **[give it a star](https://github.com/eramitgupta/world-holidays-data)** — it means a lot!

---

A **free, open-source** dataset of public holidays for **493 countries**, covering **2015 to 2059** (45 years).
Organized in a clean, developer-friendly folder structure — ready to use in any app, API, or data pipeline.

### ✨ Why Use This?

- 🌐 **Global Coverage** — 493 countries and territories
- 📅 **45 Years of Data** — 2015 to 2059
- 📂 **Clean Structure** — `holidays/{country}/{year}/holidays.json`
- 🆓 **Free & Open Source** — MIT licensed
- ⚡ **No setup needed** — just fetch the JSON directly
- 🔌 **Works everywhere** — any language, any framework

---

## 📁 Folder Structure

```
holidays/
  {COUNTRY_CODE}/
    {YEAR}/
      holidays.json
countries.json
```

### Example

```
holidays/
  US/
    2025/
      holidays.json
  IN/
    2025/
      holidays.json
countries.json
```

---

## 📄 File Formats

### `holidays/{country}/{year}/holidays.json`

```json
[
  {
    "date": "2025-01-01",
    "holiday": "New Year's Day"
  },
  {
    "date": "2025-07-04",
    "holiday": "Independence Day"
  }
]
```

### `countries.json`

```json
[
  { "code": "US",  "full_name": "United States" },
  { "code": "IN",  "full_name": "India" },
  { "code": "AE",  "full_name": "United Arab Emirates" }
]
```

---

## 🚀 How to Use

### Option 1 — Clone the repo

```bash
git clone https://github.com/eramitgupta/world-holidays-data.git
```

Then read any file directly:

```bash
cat holidays/US/2025/holidays.json
```

### Option 2 — Fetch via raw GitHub URL

```
https://raw.githubusercontent.com/eramitgupta/world-holidays-data/main/holidays/IN/2026/holidays.json
```

### Option 3 — Use in JavaScript / Fetch API

```js
const res = await fetch(
  'https://raw.githubusercontent.com/eramitgupta/world-holidays-data/main/holidays/IN/2026/holidays.json'
);
const holidays = await res.json();
console.log(holidays);
```

### Option 4 — Use in PHP

```php
$json = file_get_contents(
  'https://raw.githubusercontent.com/eramitgupta/world-holidays-data/main/holidays/IN/2026/holidays.json'
);
$holidays = json_decode($json, true);
```

---

## 📊 Stats

| Item | Value |
|---|---|
| 🌍 Countries | 493 |
| 📅 Years covered | 2015 – 2059 (45 years) |
| 🗂 Total JSON files | ~22,000+ |

---

## ⚠️ Known Limitations

- **India (`IN` / `IND`)** — Holidays available only from 2001–2035 (library limitation)
- **Marshall Islands (`MH` / `MHL`)** — Holidays available from 2020 onwards only

---

## 📝 License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

---

## 🤝 Contributing

Contributions are welcome! See [CONTRIBUTING.md](https://github.com/eramitgupta/world-holidays-data/blob/main/CONTRIBUTING.md) for guidelines.

---

## 🔗 Repository

👉 **[https://github.com/eramitgupta/world-holidays-data](https://github.com/eramitgupta/world-holidays-data)**

---

<p align="center">
  Made with ❤️ &nbsp;·&nbsp; <a href="https://github.com/eramitgupta/world-holidays-data/stargazers">⭐ Star this repo</a> &nbsp;·&nbsp; <a href="https://github.com/eramitgupta/world-holidays-data/issues">🐛 Report Bug</a> &nbsp;·&nbsp; <a href="https://github.com/eramitgupta/world-holidays-data/issues">💡 Request Feature</a>
</p>
