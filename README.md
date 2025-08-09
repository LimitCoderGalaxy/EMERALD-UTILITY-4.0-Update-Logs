# EMERALD UTILITY 4.0


## Features

- Modern Discord bot for server management, economy, achievements, moderation, and more
- Multi-currency support (coins, gems, stardust, crystals, plasma, nebula, quantum, vortex, aurora, cosmic)
- Advanced logging, daily backups, and global command cooldowns
- Modern ephemeral replies using `flags: 64` for privacy (Discord.js v14+)
- Automatic data initialization for new members (levels, balances, inventory, achievements, todos, AFK)
- Welcome message sent to a configurable channel when a new member joins



# Change Log

## v4.0.5 (2025-08-09)
- Added automatic join message: new members are welcomed in the specified channel and all user data files are initialized on join
- All ephemeral replies now use `flags: 64` (Discord.js v14+), fully removing deprecated `ephemeral` usage and warnings
- General code cleanup and modernization for Discord.js v14+ compatibility


## v4.0.4 (2025-07-06)
- Upgraded to latest `discord.js` version for all features and security updates
- Verified and updated `/say` command for full compatibility with new Discord.js enums and channel types
- All moderation and utility commands now fully compatible with Discord.js v14+ and above
- General dependency and compatibility maintenance

## v4.0.3 (2025-07-06)
- Replaced all deprecated `ephemeral: true/false` usage with `flags: 64` for Discord.js v14+ compatibility (fixes warning)
- Updated `/say` command to use only `flags: 64` for ephemeral replies and admin feedback
- Verified all moderation and utility commands for modern ephemeral usage
- General compatibility and code cleanup for Discord.js v14+

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

# Discord.js v14+ Compatibility

- All ephemeral replies now use `flags: 64` instead of `ephemeral: true/false` (required for Discord.js v14+)
- All commands and event handlers updated to use Discord.js v14 enums and APIs
- No deprecated warnings or usage remain

# Bug Fixes

- Fixed ReferenceError and undefined/null errors in `achievements.js`
- Fixed leaderboard bug with `.setDescription()`
- Fixed data format mismatch in `balances.json` for multi-currency
- Removed deprecated `fetchReply` and `ephemeral` usage
- Fixed missing import and category logic in achievements
- Fixed permission checks in `/purge` and `/roleinfo`
- Fixed help menu to remove `/balance`, `/afk`, `/unafk`, `/backup`, and `/poll` and reflect new commands
