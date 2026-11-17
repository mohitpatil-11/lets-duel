# Let’s Duel

A free, fast physics duel game that runs in your browser and installs on your phone (PWA).
Your weapon spins on its own. Tap **FIRE** when the dotted aim line points at an enemy. Every shot pushes you back and changes your spin.

**Play:** https://mohitpatil-11.github.io/lets-duel/

## Features
- 1 player vs bots (3 difficulties), 2 players on one device, free-for-all with 3 or 4 guns, and online play (host / join with a 4-letter code or invite link)
- 20+ weapons in four grades: **Special > Grade 1 > Grade 2 > Grade 3**, each with its own ability (shield blocks, rocket explodes, boomerang returns, taser stuns, cryo slows, railgun pierces, blackhole pulls, and more)
- 3 maps with different gravity: Arena, Moon, Jupiter
- Works offline after the first load (except online play); installable on Android and iPhone

## How online play works
Online matches are peer-to-peer (WebRTC through PeerJS). The host's device runs the game and sends the state to the other players.
A free PeerJS server helps devices find each other, and a TURN relay (Metered) is used when a direct connection is not possible.
Because the connection is peer-to-peer, other players can technically see your IP address. See `privacy.html`.

## Run it yourself
It is plain HTML, CSS and JavaScript. Open `index.html` in a browser, or host the folder on any static host (for example GitHub Pages).
For online play across different networks, put your Metered API key in `config.js` (`meteredKey`).

## Files
- `index.html` – the whole game
- `config.js` – your private settings (TURN key)
- `sw.js`, `manifest.json`, `icon-*.png` – offline support and installable app
- `privacy.html` – privacy notice

## Credits and notice
Inspired by *Pistol Duel* by Kayac. This is an unofficial fan project and is not affiliated with or endorsed by Kayac. No assets from the original game are used: all graphics are drawn with code and all sounds are generated in the browser.

## License
Choose a license before you share the code (for example MIT) and add a `LICENSE` file.
