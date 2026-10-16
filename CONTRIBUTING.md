# Contributing to the sirargon.net Wiki

This private repository holds player-facing Markdown. The Nuxt app lives in
`mc-network/apps/wiki`. Follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## Propose a change

Use the private [issue tracker](https://github.com/sirargonNet/wiki/issues) for
questions, corrections and topic requests. Report security problems through
[SECURITY.md](SECURITY.md).

## Local setup

Use the Node and pnpm pins in `.nvmrc` and `package.json`:

```bash
git clone git@github.com:sirargonNet/wiki.git
cd wiki
pnpm install
pnpm check
```

See the README for previewing the working tree in the monorepo app.

## Content review

- Verify gameplay facts against the monorepo and update [SOURCES.md](SOURCES.md).
- Change the German original and the English translation in the same PR.
- Keep slugs identical and use `title`, `description` and `icon` frontmatter.
- Use short, direct language; never mention another Minecraft network or server.
- Keep unknown material clearly marked as work in progress.
- Run `pnpm check` and preview both languages in the app.

## Branches and releases

Branch from `dev` and target `dev`. Conventional Commits are enforced by
commitlint; keep Husky hooks active. New player topics use `feat:`, corrections
use `fix:`. `dev` is promoted into `main` with a merge commit. The release-please
workflow publishes version tags after its release PR is merged, as described in
the README.

## Rights

Contributions remain proprietary. Do not redistribute content from this private
repository without permission.
