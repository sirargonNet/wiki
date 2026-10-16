# Content evidence

Sources are in the private `mc-network` monorepo, reviewed against commit
`d4b654669bd8e54e8e12f14d40a9d617c2768016` on the website feature worktree.
Both language trees use the same evidence. This file is editorial metadata and
is outside the published `docs/` source.

| Wiki topic                                               | Monorepo evidence                                                                                                                                                                                                                     |
| :------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Connecting, Java versions                                | `packages/app-base/app/utils/site.ts`, `apps/www/i18n/locales/{de,en}/join.json`                                                                                                                                                      |
| SMP, Creative, development status                        | `apps/www/i18n/locales/{de,en}/modes.json`, `apps/www/app/utils/modes.ts`                                                                                                                                                             |
| Friends, party, clans, voice, Discord, official modpack  | `apps/www/i18n/locales/{de,en}/community.json`, `apps/www/app/utils/community.ts`                                                                                                                                                     |
| Friends and party syntax                                 | `packages/minecraft/plugins/velocity/network/src/main/java/de/sirargon/proxy/social/{SocialCommands,SocialCommandInput}.java`, `packages/lang/locales/{de,en}/social.json`                                                            |
| Direct messages, replies, blocking, offline confirmation | `packages/minecraft/plugins/velocity/network/src/main/java/de/sirargon/proxy/chat/{ChatCommands,OfflineDirect}.java`, `packages/lang/locales/{de,en}/social.json`                                                                     |
| Clan commands and role restrictions                      | `packages/minecraft/plugins/paper/account/src/main/java/de/sirargon/account/ClanCommands.java`, `packages/lang/locales/{de,en}/clan.json`                                                                                             |
| Account, profiles, settings, XP, currencies              | `packages/minecraft/plugins/paper/account/src/main/java/de/sirargon/account/AccountMenus.java`, `packages/minecraft/plugins/paper/account/src/main/resources/lang/{de,en}/account.json`, `packages/lang/locales/{de,en}/economy.json` |
| FAQ                                                      | The same sources above; no separate gameplay assumptions                                                                                                                                                                              |
| Server rules                                             | No approved player rules found in the supplied sources; explicitly a placeholder                                                                                                                                                      |

Command tables include player actions only. Party leadership and clan membership
roles are player roles; team and moderation commands are excluded. The menus and
command registrations, rather than permission guesses, determine each entry.
Do not infer prices, rewards, limits, rules or availability from internal systems.
