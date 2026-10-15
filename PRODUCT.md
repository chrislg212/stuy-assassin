# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

A friend group in Stuy Town (the Manhattan apartment complex) playing Assassin. Each player uses their own phone, usually one-handed, often in the same room as the others while the game is being set up. The host is the friend who creates the room and presses Start. Everyone else joins with a code and opens their target in private.

## Product Purpose

Deal secret Assassin targets fairly. Each player gets exactly one target, and together the targets form a single loop, so everyone hunts one person and is hunted by one person. Success means the whole group has their target within minutes, nobody can find out anyone else's target, and the game then plays out in person without the app.

## Positioning

No accounts, no game server, and no trusted moderator. The host's phone shuffles the players and encrypts each target to the recipient's own device key (ECDH P-256 + AES-GCM). A public relay carries only sealed boxes, so even the host never sees the pairings.

## Operating Context

- Flow: enter a name, then create a room (which generates a 4-letter code) or join one with a code. The lobby fills live. The host starts once there are 3 to 20 players with no duplicate names. Each player taps to reveal their target, and the host panel shows who has received theirs.
- Players reveal their targets with other people nearby, so the screen must stay safe to glance at until the player chooses to reveal.
- `#test` puts the app in test mode, where each tab counts as a separate player for local testing.
- Players have about 12 hours to open the page and get their target, which is the relay's retention window.

## Capabilities and Constraints

- Scope is assignment only. Elimination tracking, target hand-off, leaderboards and winners are out of scope, because the game itself happens in person.
- The app must stay a single static `index.html` with no build step or framework.
- No accounts and no server: ntfy.sh (`stuytown-assassin-v1-<code>` topics) is the only relay, and the game state is rebuilt from its message log.
- The pairings stay private. Nobody, including the host, can see the full who-hunts-whom map, and only sealed boxes ever leave the host's device.
- A target is tied to the device that joined. Rejoining from another phone cannot open it.
- The room holds 3 to 20 players. Names are up to 20 characters, and room codes are 4 letters with ambiguous ones left out.

## Brand Commitments

- The name **Stuy Town Assassin** is fixed.
- The voice is plain and direct, with light spy framing (Agent, Your target, mission language). Instructions are short and practical.
- Visual stance (chosen 2026-10-14): the spy-app category standard played straight, at Valorant / Riot client polish. Dark night palette, cyan and red accents, condensed display type, a crosshair reticle. It must feel like receiving a real mission. It must never read as a hacker terminal (code rain, fake command lines), never return to the old paper-dossier look, and never get in the way of joining fast in a noisy room.
- Keep from the original: the name and title "Stuy Town Assassin", and the redaction bar over the hidden target.

## Evidence on Hand

- The live app is `index.html`. There are no testimonials, usage numbers, screenshots or logo assets, and none should be invented.

## Product Principles

1. Secrecy comes first. No pairing leaks to any screen, log, or person, including the host.
2. It should take seconds to join. That means a name and a code, with no signup and no install.
3. The app is built for one phone in one hand, in a room full of people who might peek.
4. The app deals the targets and then gets out of the way. The game happens in real life.
5. It stays a single file. Anyone should be able to host it anywhere.
