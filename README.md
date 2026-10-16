<div align="center">

# 📖 sirargon.net Wiki

**The multilingual player handbook for sirargon.net — content, translations and releases in one place**

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
- Git tags preserve each published wiki edition; `main` supplies the upcoming edition.
- No undocumented gameplay promises: [SOURCES.md](SOURCES.md) maps topics to their evidence.

## 🚀 Setup

Use the Node and pnpm versions declared in `.nvmrc` and `package.json`. Installation activates Husky. `pnpm check` checks formatting, lint, TypeScript and policy parity.

To preview **uncommitted** content, run the wiki app from a sibling `mc-network` checkout. Copy `apps/wiki/.env.example` to `apps/wiki/.env` there and point its content setting at this repository's absolute checkout path. Then:

```bash
pnpm --filter @mc-network/wiki dev
```

Open <http://localhost:3003>. Local sourcing needs neither a token nor a Git fetch and shows the working tree as upcoming `main`. It does not fabricate historical releases. The app's `.env.example` owns the configuration keys.

## 🌍 Content and languages

German (`de-DE`) lives directly in `docs/`; English lives at the same paths in `docs/en/`. Keep numeric prefixes and slugs identical, translating `title`, `description` and prose. Every page carries `title`, `description` and a Lucide `icon` in YAML frontmatter. The renderer supplies the page heading, so omit a duplicate body H1.

The consuming duxt source explicitly lists `de-DE`, `en-GB` and `en-US`. Its default locale is `de-DE`; both English source entries point at `docs/en`, so they share a full translation without a missing-translation banner. The interface still uses the selected English region. Links use absolute **content** paths such as `/guides/account`; duxt adds locale and version prefixes.

Write short, direct sentences and address the player as “du” in German. Verify facts in the monorepo before adding them. Never name another Minecraft network or server. Mark unknown material clearly as **In Arbeit / Work in progress**; the rules page is deliberately such a placeholder.

## 🤝 Contributing

Keep German and English changes together. Run `pnpm check`, then preview both languages in the consuming app; its build validates content collections and internal links. Follow [CONTRIBUTING.md](CONTRIBUTING.md). This is a private repository.

## 🛣️ Versioning

Wiki versions describe **documentation editions**, not Minecraft client versions. The manifest starts at `0.0.0`; no release or tag is created by this initial setup.

1. Merge reviewed Conventional Commits through `dev` into `main`. Use `feat:` for a new wiki capability/topic and `fix:` for a correction; docs-only commits may not trigger a release. Promote with a merge commit so release-please can see the individual commits.
2. The existing release-please workflow opens the release PR. Review its changelog and version, then merge that PR.
3. release-please publishes a GitHub release and a `vX.Y.Z` Git tag. Never move a published tag; correct content in a new release.
4. Rebuild/redeploy `apps/wiki` to discover the new tags. duxt reads all release tags, selects the newest as the default and retains older editions. `main` is labelled upcoming.

> [!IMPORTANT]
> The first remote app build with release discovery needs at least one released tag containing `docs/`. Before that, use the local source. The private repository also needs build-time read credentials, and the existing release workflow needs its configured CI secret and write permissions. No credentials belong in Markdown.

## 📄 License

Proprietary. All rights reserved. Access to this private repository does not grant permission to redistribute its contents.
