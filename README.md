> [!WARNING]
> **SF4Enhanced is no longer maintained**, and this repository is archived.
>
> The last build and the source code are at
> [fabeloper/sf4e](https://github.com/fabeloper/sf4e/releases/latest). The public lobby servers
> stay online for the people who still play on them, with no promise of how long. For actively
> developed rollback netplay in Ultra Street Fighter IV, use
> [SF4 Ember Netplay](https://github.com/Confetti3/SF4-Ember-Netplay).

# SF4Enhanced

**Rollback netcode for Ultra Street Fighter IV (Steam).**

Play USF4 online with modern rollback netcode, lobby codes, and spectating —
no port forwarding, no sharing IPs.

➡️ **[Download the latest release](../../releases/latest)**

---

## What it is
A mod that adds GGPO-style rollback netcode to the Steam release of
Ultra Street Fighter IV, plus an online lobby system:

- **Rollback netcode** instead of the original delay-based netplay
- **Lobby codes** — share a 6-character code, no IP addresses
- **Choose your server** — Spain or Germany, pick whichever is closer
- **Spectator mode**
- **Adjustable input delay**

## Requirements
- **Windows**
- **Ultra Street Fighter IV on Steam** — you must own the game. This mod does
  not include the game and will not work without it.

## Install
1. Download the `.zip` from the [latest release](../../releases/latest)
2. Unzip it anywhere
3. Run `SF4Enhanced.exe`

If Windows SmartScreen warns you, choose **More info → Run anyway**. The build
is unsigned; a code-signing certificate costs money this project does not have.

## ⚠️ Important: both players must use the same frame-rate setting
In the game's graphics options, set **"frames per second" / "imágenes por
segundo"** to **Variable**, and make sure **both players use the same value**.

Mismatched settings make each machine advance the intro animation by a different
amount, which desyncs the match within seconds. This is the single most common
cause of desyncs.

## Status: BETA
This is a work in progress, tested by a small group. Expect rough edges:

- Rare desyncs can still happen around knockouts / round transitions. When one
  is detected the match ends cleanly and tells you, rather than silently
  drifting apart.
- Rare crashes are still being investigated.
- Both players must pick the **same server**; lobby codes live on one server.
- Tested with a handful of players so far — your mileage may vary.

If something breaks, the log at `%APPDATA%\sf4e\logs\sf4e.log` is what makes it
fixable.

## Disclaimers
- **Not affiliated with, endorsed by, or associated with Capcom.** Street
  Fighter and Ultra Street Fighter IV are trademarks of Capcom. This is an
  unofficial, non-commercial fan project.
- **No game assets are included or distributed.** You must own a legitimate copy
  of the game on Steam.
- **Use at your own risk.** This mod injects into the game process. It is
  provided as-is, with no warranty of any kind. It is intended for private play
  with friends, not for ranked or official online modes.
- Built on the [sf4e](https://codeberg.org/adanducci/sf4e) project.

## Credits
Built on **sf4e** by adanducci, which did the original reverse-engineering and
rollback groundwork. This distribution packages that work with an online lobby
system and hosted servers.
