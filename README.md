# EMERALD UTILITY 4.0


# Change Log

## v4.0.2 (2025-06-27)
- Modernized all moderation and protection commands: `/addlevel`, `/removelevel`, `/clear`, `/lockdown`, `/lockserver`, `/antiraid`, `/antispam`, `/automod`, `/joinfilter`, `/mentionprotect`, `/raidprotection`, `/raidmode`, `/audit`
- All moderation actions now use embeds with moderator, timestamp, and detailed configuration/status
- Improved error handling and audit logging for all moderation/protection commands
- Consistent ephemeral replies for privacy and transparency
- General code cleanup and modernization for maintainability

## v4.0.1 (2025-06-26)
- Added 20 new achievements: expanded `currency_collector`, `wealth_milestones`, and introduced `spender_milestones` for spending achievements
- `/achievements view` now dynamically lists all categories and new achievements automatically
- Improved `/achievements` command: ephemeral replies, user tag and timestamp in embed, better error handling
- Cleaned up unused AFK files: deleted `afk.json` and `afkStatus.json`
- General code and data cleanup for removed AFK features

## v4.0.0 (2025-06-25)
- Removed deprecated `/balance` command (use `/currency balance` instead)
- Added multi-currency support and fixed balances data format
- Improved `/currency` command (balance, convert, list)
- Added DM support for many commands
- Added global command cooldown and advanced logging
- Fixed leaderboard and achievements bugs
- Updated help menu to reflect current commands
- Added progress bar and percentage to `/level` command
- Added level-up rewards: users now earn EchoBucks for leveling up, with special bonuses every 5 levels
- Removed `/afk`, `/unafk`, `/backup`, and `/poll` commands and cleaned up help menu
- Improved `/deposit` and `/withdraw` commands: support for "all", input validation, multi-currency, and privacy
- Enhanced `/work` command: now randomly rewards one of your currencies (EchoBucks, gems, stardust, crystals, plasma, nebula, quantum, vortex, aurora, cosmic) each time you work, with unique reward ranges and updated embed
- Upgraded `/rob` and `/coinflip` commands: multi-currency, input validation, privacy, and better feedback
- Upgraded `/serverinfo` command: more details and embed
- Updated `/ping` command: added ephemeral option, dynamic user/time, and privacy support
- Updated `/say`, `/daily`, `/craft`, `/inventory`, `/roleinfo`, and `/8ball` commands: dynamic timestamp, user tag in footer, privacy improvements, and ephemeral replies
- Removed `/poll` command and all references from help/documentation
- Updated all ephemeral replies to use `flags: MessageFlags.Ephemeral` for Discord.js v14+ compatibility

# Bug Fixes

- Fixed ReferenceError and undefined/null errors in `achievements.js`
- Fixed leaderboard bug with `.setDescription()`
- Fixed data format mismatch in `balances.json` for multi-currency
- Removed deprecated `fetchReply` and `ephemeral` usage
- Fixed missing import and category logic in achievements
- Fixed permission checks in `/purge` and `/roleinfo`
- Fixed help menu to remove `/balance`, `/afk`, `/unafk`, `/backup`, and `/poll` and reflect new commands
