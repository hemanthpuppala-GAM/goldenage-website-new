# Contributing

Thank you for helping with the Golden Age Wisdom site. This page is the whole
process — it is short on purpose.

## The two branches

| Branch | What it is |
|---|---|
| `main` | The live site. Protected. Nothing reaches it without review. |
| `staging` | Where work happens and gets tested. Push here freely. |

## Making a change

1. Open the file on the **`staging`** branch — check the branch dropdown says
   `staging`, not `main`.
2. Click the pencil icon, make your edit.
3. At the bottom choose **Commit directly to the staging branch**, write a short
   message saying what you changed and why, and commit.
4. Check your change on the staging copy of the site before going further.

## Getting it live

1. Go to the **Pull requests** tab → **New pull request**.
2. Set base `main`, compare `staging`.
3. Describe what changed and what you tested it on — which pages, which screen
   sizes, and whether you checked a phone.
4. Create the pull request. The maintainer reviews it.
5. Once approved and merged, the maintainer uploads the changed files to the
   server.

## Things worth knowing

- **`sw.js` must be uploaded whenever any page changes**, with its version
  constant bumped. It caches the site, so without it visitors keep seeing the
  old page and your work appears to have done nothing.
- **Colour** — the palette is fixed. If a colour you need is not already in the
  site, raise it before using it rather than inventing a hex value.
- **Type** — Marcellus for display, Outfit for body, Noto Sans for Telugu and
  Devanagari.
- **Copy** lives in `gaw-i18n.js`, not in the pages. Change it there so every
  language stays in step.
- **Never commit** member data, form submissions, API keys or passwords.

## If something breaks on the live site

Tell the maintainer straight away with the page, the device, and a screenshot.
Do not push a fix directly to `main` — the review exists to stop one urgent fix
becoming two problems.
