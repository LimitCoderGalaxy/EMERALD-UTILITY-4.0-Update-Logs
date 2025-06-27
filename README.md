# EMERALD UTILITY 4.0


# Change Log

## v4.0.0 (2025-06-27)
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
- Enhanced `/work` command: now randomly rewards one of your currencies (EchoBucks, gems, stardust, etc.) each time you work, with unique reward ranges and updated embed
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
