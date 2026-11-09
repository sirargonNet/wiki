<div align="center">

# 📖 sirargon.net Wiki

**The multilingual player handbook for sirargon.net — content and translations in one place**

</div>

---

```bash
pnpm install
pnpm check
```

Edit Markdown in `docs/`. The website lives in the private `mc-network` monorepo at `apps/wiki`; this repository only owns content and its quality tooling.

## ✨ Features

- First steps, game modes, friends, parties, clans, voice chat and your account.
- German originals and a complete English translation shared by both English regions.
- One unversioned edition: the website always shows `main`.
- No undocumented gameplay promises: `apps/wiki/SOURCES.md` in the monorepo maps topics to their evidence.

## 🚀 Setup

Use the Node and pnpm versions declared in `.nvmrc` and `package.json`. Installation activates Husky. `pnpm check` checks formatting, lint, TypeScript and policy parity.

To preview **uncommitted** content, run the wiki app from a sibling `mc-network` checkout. Copy `apps/wiki/.env.example` to `apps/wiki/.env` there and point its content setting at this repository's absolute checkout path. Then:

```bash
pnpm --filter @mc-network/wiki dev
```

Open <http://localhost:3003>. Local sourcing needs neither a token nor a Git fetch and shows the working tree. The app's `.env.example` owns the configuration keys.

## 🌍 Content and languages

German (`de-DE`) lives directly in `docs/`; English lives at the same paths in `docs/en/`. Keep numeric prefixes and slugs identical, translating `title`, `description` and prose. Every page carries `title`, `description` and a Lucide `icon` in YAML frontmatter. The renderer supplies the page heading, so omit a duplicate body H1.

The consuming duxt source explicitly lists `de-DE`, `en-GB` and `en-US`. Its default locale is `de-DE`; both English source entries point at `docs/en`, so they share a full translation without a missing-translation banner. The interface still uses the selected English region. Links use absolute **content** paths such as `/guides/account`; duxt adds locale prefixes.

Write short, direct sentences and address the player as “du” in German. Verify facts in the monorepo before adding them. Never name another Minecraft network or server. Mark unknown material clearly as **In Arbeit / Work in progress**; the rules page is deliberately such a placeholder.

## 🤝 Contributing

Keep German and English changes together. Run `pnpm check`, then preview both languages in the consuming app; its build validates content collections and internal links. Follow [CONTRIBUTING.md](CONTRIBUTING.md). This is a private repository.

## 🛣️ Publishing

The wiki is not versioned: there are no release tags and no version switcher. Merge reviewed Conventional Commits through `dev` into `main`; the `Content bundle` workflow packs `main` with the content packer of the release in production and uploads it, and the website loads it within about a minute. Its required variables and secrets are listed at the top of `.github/workflows/content-bundle.yml`.

## 📄 License

Proprietary. All rights reserved. Access to this private repository does not grant permission to redistribute its contents.
