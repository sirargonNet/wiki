# CLAUDE.md

Guidance for agents working on the private sirargon.net player wiki.

## Agent files

`CLAUDE.md` and `AGENTS.md` are byte-identical real files. After editing one,
copy it wholesale over the other; never repeat the edit by hand.

## Scope

This is a content-only repository. Markdown lives in `docs/`; the website is
`apps/wiki` in the private `mc-network` monorepo. Do not add Nuxt or runtime
packages here. Read `README.md`, `SOURCES.md` and `CONTRIBUTING.md` first.

## Content

- German (`de-DE`) is the default tree at `docs/`. English is `docs/en/`, shared
  by `en-GB` and `en-US`. Every German page change includes its English counterpart
  at the identical slug and numeric prefix.
- Frontmatter has `title`, `description` and `icon`. Do not duplicate the title
  as a body H1. Use absolute content links; duxt supplies version/locale prefixes.
- Verify every gameplay claim against the monorepo. `SOURCES.md` records evidence.
  Unknown material is explicitly “In Arbeit / Work in progress”, never invented.
- Address players as “du”; write short, direct sentences. Never name another
  Minecraft network or server anywhere. Comments are English.
- Player command lists exclude team and moderation commands. Do not infer
  permissions, rewards, prices or gameplay availability.

## Tooling

- Follow `.nvmrc` and `package.json` runtime/package-manager pins. Dependencies
  stay pinned; the three-day release cooldown remains enabled.
- `pnpm install` activates Husky. `pnpm check` runs lint, format, TypeScript and
  policy parity. Do not bypass hooks. `pnpm check:fix` fixes lint/format.
- Workflows call pinned shared kirchDev bodies; do not copy their implementation.
- This repository is private: no LICENSE, CodeQL workflow or issue-template
  Discord contact links. Contributions and content are proprietary.
- Keep `.claude/settings.json` and `.codex/rules/default.rules` command bans in
  sync; `pnpm check:policy` verifies parity. Never allow arbitrary execution.

## Versions

`release-please-config.json` and `.release-please-manifest.json` own release
metadata. Wiki tags version the content, not Minecraft. Branch from `dev`, target
`dev`, promote into `main` with a merge commit. Never rewrite a published tag.
No commit, push, tag or release action is implied by a content-editing request;
follow the session's explicit authorization.
