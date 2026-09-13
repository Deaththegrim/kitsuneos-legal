# kitsuneos-legal

Public source for the **KitsuneOS** Privacy Policy and Terms of Service, served by GitHub
Pages. The game's own repository is private, and GitHub Pages cannot serve from a private
repository on the free plan — which is why these two documents live in their own repo.

| Document | URL |
|---|---|
| Privacy Policy | https://deaththegrim.github.io/kitsuneos-legal/privacy/ |
| Terms of Service | https://deaththegrim.github.io/kitsuneos-legal/terms/ |

Both URLs are set in the Discord Developer Portal for the KitsuneOS application.

## Editing

`privacy.md` and `terms.md` are plain Markdown with Jekyll front matter; the `permalink`
field fixes each URL, so **don't change it** — the Developer Portal points at those paths.
`_layouts/default.html` holds the styling and is self-contained (no theme gem), so the Pages
build has no external dependency to break.

Push to `main` and Pages rebuilds. Update the `updated:` date in the front matter whenever
the text changes materially.

The Privacy Policy describes what the game actually does. If the game starts collecting
something new — a new stored field, a new upload path, an off-site backup, anything
third-party — update the policy in the same change.
