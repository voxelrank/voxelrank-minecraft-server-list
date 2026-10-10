# VoxelRank – server list for Minecraft and 11 other games

[VoxelRank](https://voxelrank.com) is a free server list where the ranking comes from player votes. You can't buy a higher rank. Sponsored slots exist, but they are always labelled and sit apart from the vote ranking.

This repo holds docs and setup guides for server owners.

## Games

Minecraft (Java, Bedrock, cross-play), Hytale, Rust, ARK, GTA V (FiveM), GTA VI, CS2, Valheim, Terraria, Palworld, DayZ and Discord communities.

The site is translated into 26 languages.

## For server owners

### Add your server

1. Go to [voxelrank.com/add](https://voxelrank.com/add).
2. Enter the address. We ping it, then fill in the version, player count and icon.
3. Add tags, a description and a banner (an image, a GIF, or a short video we convert for you).

Listing a server is free.

### Vote rewards in game (Minecraft)

There are two ways to give players rewards for voting:

- **The VoxelRank plugin** (Spigot, Paper, Purpur and Folia, Minecraft 1.8.8 and newer, Java 8+). Download it from [voxelrank.com/download/plugin](https://voxelrank.com/download/plugin). By default it fetches votes over HTTPS with your API key, so you don't need to open a port. It catches up on votes missed while the server was offline.
- **NuVotifier / Votifier** (v1 and v2). Fill in your Votifier details on your listing and each vote is pushed to your server as it happens.

You can also use both: Votifier for instant delivery, with the plugin as a backup. Each vote is only delivered once.

### Badges and banners for your site

Show your live status and votes on your website or forum:

```markdown
[![VoxelRank](https://voxelrank.com/banner/YOUR-SLUG/badge.svg)](https://voxelrank.com/server/YOUR-SLUG)
```

Replace `YOUR-SLUG` with the slug from your server's address. You can find more banner styles and ready-made embed codes in your listing's owner tools under **Promote & rewards**.

A verified, followed link back to your listing also gets you a free bump every 12 hours instead of every 24.

## For players

- Filter servers by game, version, mode, region and language.
- Vote in a few seconds, no account needed.
- Read reviews from players who voted for that server.

## Links

- Website: https://voxelrank.com
- Add a server: https://voxelrank.com/add
- Questions or bugs: open an issue in this repo.

## License

MIT
