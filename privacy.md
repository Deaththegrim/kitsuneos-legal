---
layout: default
title: Privacy Policy
permalink: /privacy/
updated: 14 September 2026
---

KitsuneOS is a free Discord game, operated by **Deaththegrim** ("the operator", "we").
It runs as a Discord bot and a Discord Activity inside servers that have invited it.

This policy explains exactly what the game stores, why, where it lives, and how to get it
removed. It describes what the software actually does — not a generic template.

## 1. What KitsuneOS stores

### Account and gameplay data

When you first use a KitsuneOS command, the game creates a record for you:

| Data | Why |
|---|---|
| Your Discord **user ID** (the numeric ID, not your password or email) | Identifies your save |
| The **server (guild) ID** you are playing in | Saves are per-server; your progress in one server is separate from another |
| Gameplay state — trainer level, experience, currency, inventory, gear, collected effigies, battle and trade records, unlocks | It is the game |
| Timestamps — when you started, and cooldown stamps for actions like exploring | Enforces cooldowns and seasons |

### Data derived from server members

KitsuneOS builds its roster from the members of the server it is in. When it scans a server —
on start-up, when someone joins, or when a moderator runs the scan command — it stores, for
each member:

- the member's **Discord user ID**
- the member's **display name at the time of the scan**, which becomes the name of an
  in-game "effigy"
- the **URL of the member's Discord avatar**, and whether that avatar is animated
- game attributes derived from the above (an element type, an archetype, and statistics)

**Members scanned this way are not catchable by other players by default.** A scanned effigy
is created in a non-catchable state and is hidden from the in-game browser and its search
until that member opts in themselves. Opting in is done by the member and no one else.

If you are in a server with KitsuneOS and you would rather not appear at all, see
[Your choices](#5-your-choices) below.

### Content you submit

- **Character submissions and artwork.** If you submit a character or add artwork, the image
  file is downloaded and stored on the game's server, and is resized. Discord's own
  attachment links expire, which is why the file is kept rather than linked.
- **Feedback.** The in-game feedback command stores the text you write, your user ID, and
  the server ID, so the operator can read and act on it.

### The Discord Activity

The in-Discord Activity asks Discord for authorisation using the scopes `identify`, `guilds`,
`applications.commands` and `rpc.activities.write`. The game's server performs the token
exchange so that the client secret is never exposed to your browser.

**The resulting access token is not stored.** It is handed straight back to the Activity
running in your Discord client, which sends it with each request so the server can confirm
who you are. Nothing about the token is written to disk or to the database.

## 2. What KitsuneOS does not collect

- **No email addresses**, real names, or postal addresses.
- **No payment details.** The game is free and has no purchases of any kind (see the
  [Terms of Service]({{ '/terms/' | relative_url }})).
- **No message content.** The bot does not have Discord's Message Content intent enabled. It
  cannot read your conversations, and does not store them.
- **No direct messages and no voice data.**
- **No analytics, advertising, or third-party tracking of any kind.** There are no ad
  networks, no trackers, and no cookies set for advertising.

## 3. Where the data lives

Game data is held in a single database file on a virtual machine rented from **Oracle Cloud**,
located in the **Melbourne, Australia** region. Uploaded artwork is stored as files on that
same machine. Backups are kept on that server; if off-site backups are enabled in future,
they would go to a third-party storage provider and this policy will be updated to say so.

Discord itself necessarily processes your data in order for the game to work at all — your
use of Discord is governed by Discord's own privacy policy, not this one.

## 4. Who it is shared with

**Nobody.** KitsuneOS does not sell, rent, trade, or share your data with third parties. It
is not used for advertising or profiling. The only parties with access are:

- **the operator**, who administers the server;
- **Oracle Cloud**, as the hosting provider (they hold the disk, not the game);
- **Discord**, as the platform the game runs on.

Some information is visible to other players inside your server by design — your effigy, your
collection, ladder standings, and trades are part of playing a multiplayer game.

## 5. Your choices

- **Opt in / opt out of being catchable.** Use the in-game opt-in and opt-out commands. You
  control this for your own effigy; nobody else can set it for you. Opting out stops other
  players from catching new copies of your effigy.
- **Ask for removal.** You can ask for your player record, your effigy, or artwork you
  submitted to be deleted. See [Contact](#8-contact). Removal requests are honoured.
- **Leave.** Removing the bot from a server, or leaving that server, does not by itself
  delete the data already stored — ask for removal if that is what you want.

## 6. How long it is kept

Data is kept for as long as the game is running and you have a save in it, because it *is*
your save. There is no fixed expiry. Data is deleted when you ask for it to be deleted, or if
the game shuts down permanently.

## 7. Age

KitsuneOS is played through Discord, and Discord requires its users to be at least 13 years
old (or older, where local law sets a higher minimum). The game is not directed at children
under that age, and does not knowingly keep data for anyone below it. If you believe a child
under the minimum age has a save, contact the operator and it will be removed.

## 8. Contact

Privacy questions and removal requests go through Discord:

- use the in-game **feedback command** in any server running KitsuneOS, or
- **direct-message the operator** on Discord (**Deaththegrim**).

Requests are handled by a single person running a hobby project, so allow a reasonable amount
of time for a reply.

## 9. Changes to this policy

If this policy changes, the updated version is published at this URL and the "last updated"
date at the top changes with it. Material changes will be announced in-game or in the
servers running KitsuneOS.
