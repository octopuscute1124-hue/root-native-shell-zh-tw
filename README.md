# Root — Traditional Chinese (zh-TW) Localization String Reference

A community-maintained **Traditional Chinese (zh-TW) localization string reference** for **Root**, a chat & community platform (see [docs.rootapp.com](https://docs.rootapp.com/)). The strings are extracted from Root's desktop client localization resources and distributed as a single CSV file for translators, developers, and localization tooling to use freely.

> This repository contains only the string-reference data. Its purpose is to make the zh-TW translation effort collaborative, traceable, and reusable by anyone.

---

## What's in the file

| Column | Description |
| --- | --- |
| `key` | Internal string identifier (unique key) |
| `english` | Original English string (may include format placeholders such as `{0}` and markdown markers such as `**bold**`) |
| `zh_TW` | Corresponding Traditional Chinese translation |

- File: `Root Localization String Reference (zh-TW).csv`
- Entries: **1,657**
- Encoding: UTF-8 (with BOM), CRLF line endings
- Coverage: community management, channels & voice, roles & permissions, apps/bots, the Core system, direct messages, account & security (Passkey / password / login), settings, notifications, and the rest of the UI surface.

## Use cases

- **Collaborative translation**: use this table as the baseline for zh-TW proofreading and terminology unification (e.g. 「社群」「身分組」「核心」). Use `key` as the unique identifier when splitting work across multiple people to avoid duplicates and conflicts.
- **Developer integration**: import the CSV into your project to diff against i18n resource files, or generate a Traditional Chinese language pack.
- **Quality checks**: compare `english` vs `zh_TW` to verify placeholders (`{0}`, `{1}`…) and markdown markers (`**…**`) are preserved in the translation.

## How to use

1. Download the CSV and open it in Excel / Google Sheets / Numbers (plain UTF-8 CSV, importable directly).
2. Sort or filter by `key` to review and edit translations entry by entry.
3. To use it in code, convert to your preferred format (JSON / PO / properties…). The `key` column maps directly to resource keys.

## Source & attribution

- The `key` and `english` strings are **extracted from the localization resources of Root** — a chat & community platform (docs: https://docs.rootapp.com/).
- This repository is an **unofficial, independent** reference — it is not affiliated with or endorsed by Root, and the translations are not official.
- The project deliberately ships as a **standalone CSV reference** and does not modify the application itself (modifying the app would invalidate its code signature).
- All original strings (`key` and `english`) are the property of their respective owner(s). The `zh_TW` translations are contributed by this repository's maintainers.
- If you are the copyright holder and would like this reference removed, please open an issue and we will take it down promptly.

## Notes

- Translations follow **Taiwan Traditional Chinese** conventions. Suggestions for more natural localizations are welcome.

## Contributing

Feel free to open an Issue or Pull Request:

- Fix an existing translation: point out the `key` and your suggested wording.
- Add new entries: provide `key`, `english`, and `zh_TW`.
- Keep the CSV format: `key,english,zh_TW`, UTF-8.

## License

The translation data in this repository is released under the **MIT License** — free to use, modify, and redistribute, including for commercial purposes.

See [LICENSE](./LICENSE).
