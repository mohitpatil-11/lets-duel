# Whirlshot

A fast physics duel game for the browser and phone (PWA). Your weapon spins on its own; tap **FIRE** when the aim line points at an enemy. Every shot pushes you back and changes your spin. Last one standing wins.

**Play:** https://mohitpatil-11.github.io/lets-duel/

## Features
- 1 player vs bots, 2 players on one device, free-for-all with 3 or 4 weapons, and online play (4-letter room code or invite link)
- 25 weapons in four grades (**Special > Grade 1 > Grade 2 > Grade 3**) with their own abilities
- 3 maps with different gravity: Arena, Moon, Jupiter
- Profile name, match results with kills, coins, and cosmetic skins (they never change strength)
- Works offline after the first load (except online play), installable on Android and iPhone

## Settings for a public launch (`config.js`, see `config.example.js`)
- `meteredKey` – relay key for online play across networks
- `iceServers` – your own TURN/STUN servers (recommended instead of a shared key)
- `peerServer` – your own PeerJS matchmaking server

## Files
`index.html` (the game), `config.js` (private settings), `sw.js` + `manifest.json` + icons (offline and install), `privacy.html`, `terms.html`, `LICENSE`.

## Legal
© 2026 Mohit Patil. All rights reserved (see `LICENSE`). Third-party libraries keep their own licenses.
