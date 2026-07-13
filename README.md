# taibu-docs

Public documentation for **Taibu AI OS**. The desktop app pulls these files on
launch (with an offline bundled fallback), so editing a guide here updates the
app's **Guides** and **Help** without shipping a new build.

## Structure

```
docs.json          canonical guide order (one list, language-independent)
en/                English (base language / fallback for all others)
et/                Eesti
de-DE/  de-AT/     Deutsch
ru/                Русский
<lang>/<slug>.md   same filenames across every language
```

## How it works

- `docs.json` lists the canonical slugs in display order.
- For a given user language, each slug resolves per file with a fallback chain
  (e.g. `de-AT → de-DE → en`), so a language that hasn't translated a guide yet
  still shows the English one under the same slug (never a mixed duplicate list).
- Each file's first `# H1` is used as its title in the app.

## Editing

1. Edit or add `<lang>/<slug>.md` (keep the same filename across languages).
2. New guide? Add its slug to `docs.json` `order`.
3. Commit to `main`. The app picks it up on next launch.

Keep copy simple and human. No em dashes.
