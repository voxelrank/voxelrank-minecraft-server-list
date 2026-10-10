---
title: VoxelRank owner guide – vote rewards, Votifier and badges
description: How to set up vote rewards for your Minecraft server on VoxelRank with the plugin or NuVotifier, and how to add a live badge to your website.
---

# VoxelRank owner guide

This guide is for people who run a game server and list it on [VoxelRank](https://voxelrank.com). It covers three things: rewarding players for votes, choosing between the plugin and Votifier, and showing your rank on your own site.

## 1. List your server

Go to [voxelrank.com/add](https://voxelrank.com/add) and enter your server address. We ping it and fill in the version, player count and icon for you. Then add tags, a description and a banner. Listing is free.

## 2. Reward players for voting

### Option A: the VoxelRank plugin

Works on Spigot, Paper, Purpur and Folia, Minecraft 1.8.8 and newer, Java 8 or newer.

1. Download the jar from [voxelrank.com/download/plugin](https://voxelrank.com/download/plugin) and put it in your `plugins/` folder.
2. Start the server once so the plugin creates `plugins/VoxelRank/config.yml`.
3. Copy your server's API key from your listing's owner tools and paste it into `api-key` in `config.yml`.
4. Set the reward commands under `rewards:` → `commands:`.
5. Run `/votingsite reload`. No restart needed.

The plugin fetches votes over HTTPS, so you don't need to open any port. If your server was offline when someone voted, the vote is delivered once it comes back.

Useful commands:

| Command | What it does |
|---|---|
| `/votingsite reload` | Re-reads the config |
| `/votingsite testvote <player>` | Sends a test vote, so you can check your rewards |
| `/votingsite status` | Shows the mode, whether the API key is set and how many votes were delivered |
| `/voxelrank vote` | Gives players the link to vote |
| `/voxelrank top` | Shows the top voters |

### Option B: NuVotifier / Votifier

If you already run NuVotifier (v1 or v2), enter your Votifier host, port and key on your listing. Each vote is pushed to your server the moment it happens, and any Votifier listener plugin you already use will handle it.

### Both at once

You can run both. Votifier gives instant delivery, the plugin catches anything missed. Each vote is still only delivered once.

## 3. Show your rank on your website

A live badge with your status and votes:

```markdown
[![VoxelRank](https://voxelrank.com/banner/YOUR-SLUG/badge.svg)](https://voxelrank.com/server/YOUR-SLUG)
```

Or in HTML:

```html
<a href="https://voxelrank.com/server/YOUR-SLUG"><img src="https://voxelrank.com/banner/YOUR-SLUG/badge.svg" alt="Vote for us on VoxelRank"></a>
```

`YOUR-SLUG` is the last part of your listing's address, for example `880-relxmc`. More banner styles and ready-made embed codes are in your owner tools under **Promote & rewards**.

## Questions

Open an issue in [the repo](https://github.com/voxelrank/voxelrank-minecraft-server-list/issues) or use the contact page on [voxelrank.com](https://voxelrank.com).
