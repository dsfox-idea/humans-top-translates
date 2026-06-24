# humans.top — community translations

Open translations for the **[humans.top](https://humans.top)** apps (iOS, Android)
and website. **Spotted a wrong or awkward translation? Fix it here and open a Pull
Request** — every change is reviewed and ships to the live apps and site on the
next build.

## How to contribute (no coding needed)

1. Find your language file:
   - **UI strings** (buttons, labels, screens) → [`ui/<lang>.json`](ui/)
   - **Server messages** (errors) → [`backend/<lang>.json`](backend/)
2. Edit the **value** on the right. **Never change the key on the left** — it's
   what the apps look up.
   ```json
   "signOut": "Se déconnecter",
              ^^^^^^^^^^^^^^^^^ change this
   ^^^^^^^^^ keep this
   ```
3. Open a Pull Request. That's it. We review and merge.

`ui/en.json` is the **English reference** — compare against it to see what a key
means. If a key is missing in your language, add it (copy the key from `en.json`).

## Languages (15)

`en` English · `ru` Русский · `de` Deutsch · `fr` Français · `it` Italiano ·
`es` Español · `tr` Türkçe · `zh-Hans` 简体中文 · `pl` Polski · `sr-Cyrl` Српски ·
`ar` العربية · `hi` हिन्दी · `bn` বাংলা · `pt` Português · `ja` 日本語

## Placeholders — keep them exactly

Some strings contain a placeholder that the app fills in at runtime. **Keep it in
your translation, move it where your language needs it:**

- `{n}` — a number, e.g. `"{n} left"` → `"осталось {n}"`
- `{s}` — a piece of text, e.g. `"Buy {s}"` → `"Acheter {s}"`

## Notes

- Keep it concise — these are UI labels; long text breaks layouts.
- Match the tone of the existing strings (friendly, plain).
- RTL languages (`ar`) are handled by the apps automatically — just translate.
- License: CC0 1.0 (public domain) — see [`LICENSE`](LICENSE). By contributing you
  agree your translation is released under it.

Thank you for helping make humans.top read naturally in your language. ❤️
