# Emerald Bot v26.3.1

## Highlights
- 75 active slash commands
- Full economy loop: work, daily/weekly, gambling, banking, trading
- XP, badges, titles, and VIP multipliers
- Moderation and server management toolkit
- GitHub-powered `/updates` command for live changelog previews
- Performance optimizations for cache cleanup, cooldown handling, and stable runtime behavior

## Core Systems
- Economy: currencies, balances, shop, inventory, streaks, payouts
- Leveling: message XP, level progression, title unlocks
- Badges/Titles: achievement-based unlock paths
- Moderation: warnings, notes, timeout/ban/kick, cleanup commands
- Utility: profile, leaderboards, reminders, server insight, reporting

## Featured Commands
- Economy: `/work`, `/beg`, `/daily`, `/weekly`, `/balance`, `/shop`, `/deposit`, `/withdraw`
- Gambling: `/coinbet`, `/coinflip`, `/dice`, `/slots`, `/roulette`, `/rob`, `/steal`
- Social: `/profile`, `/userinfo`, `/leaderboard`, `/leaderboardlevel`, `/titles`, `/title`
- Moderation: `/warn`, `/warnings`, `/clearwarnings`, `/note`, `/notes`, `/clearnotes`, `/timeout`, `/ban`, `/kick`, `/purge`
- Utility: `/help`, `/botinfo`, `/serverinfo`, `/ping`, `/report`, `/remind`, `/updates`
- Fun/Community: `/fun`, `/rps`, `/poll`, `/giveaway`, `/ticket`, `/rules`, `/weather`

## /updates Command
`/updates` pulls update notes from:
1. `UPDATELOG.md`
2. `CHANGELOG.md`
3. `UPDATES.md`
4. `README.md`

If no log file is found, it shows recent commits from:
https://github.com/LimitCoderGalaxy/EMERALD-UTILITY-4.0-Update-Logs

## Session Update (March 15, 2026)
- Configured report routing with `REPORT_CHANNEL_ID` in `.env`.
- Upgraded welcome flow with a modern embed (avatar, member count, timestamp, and onboarding field).
- Updated `/work` to post publicly so everyone can see earnings activity.
- Added `/updates` command to pull changelog content directly from your GitHub update-log repo.
- Redeployed slash commands and restarted the bot after command set cleanup.
- Added runtime optimization work (command load checks, cache/cooldown cleanup loop, and global error handlers).
- Refreshed this README to reflect current setup and command guidance.

## Requirements
- Node.js >= 22.12.0
- discord.js ^14.25.1
- dotenv ^17.3.1

## Version
- Current: v26.3.1 "SAPPHIRE" (March 2026)
