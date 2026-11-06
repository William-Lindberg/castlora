<div align="center">

# Castlora

**Your games. Your mistakes. Your repertoire.**

A free chess improvement app that analyses the games you have already played, right on your own device.

[**Open the web app**](https://william-lindberg.github.io/castlora/app/) · [**Download for Android**](https://github.com/William-Lindberg/castlora/releases/latest) · [Website](https://william-lindberg.github.io/castlora/)

`Free to use` · `No account` · `No ads or tracking` · `Stockfish 19 on your device`

</div>

---

## What is Castlora?

Castlora turns your own finished games into training:

| | |
|---|---|
| **Game analysis** | Stockfish 19 checks every move of your finished games, on your device. |
| **Mistake intelligence** | Blunders, mistakes and inaccuracies, sorted by theme (missed tactics, hanging pieces, missed captures, king safety, opening, endgame, calculation, positional). Retry each position, with hints. |
| **Automatic opening repertoire** | Your *played* repertoire is built strictly from moves you actually played. Next to it, you curate a separate *prepared* repertoire. |
| **Adaptive coach** | Explanations and training pitched at your level: Beginner (below 1000), Intermediate (1000–1799) or Advanced (1800+), based on your Chess.com Rapid rating (or a level you choose). These are provisional categories. |
| **Personal training** | Spaced repetition from your own mistakes and openings. |
| **Progress intelligence** | Charts and evidence-based recommendations from your own games. |
| **Opening training** | Practise your played and prepared repertoires move by move. |

Import games by **Chess.com username** (public API) or from **PGN files**. Castlora only works with **completed games** and never helps during a live game.

## Install on Android

1. On your phone, open the [latest release](https://github.com/William-Lindberg/castlora/releases/latest) and download the Castlora `.apk` file.
2. **Check the file.** Compare its SHA-256 checksum with the one in `SHA256SUMS.txt` in the same release. On a computer:
   - macOS / Linux: `shasum -a 256 Castlora-*.apk`
   - Windows (PowerShell): `Get-FileHash .\Castlora-*.apk -Algorithm SHA256`
3. Open the APK. Android asks you to allow your browser or file manager to **install unknown apps**. Allow it for that app only.
4. Install Castlora. Afterwards you can switch the "install unknown apps" permission off again.

> **Note:** Google is rolling out Android developer verification for apps installed outside the Play Store, so depending on your device and country, Android may show extra warnings or steps. Only download Castlora from this repository's [Releases page](https://github.com/William-Lindberg/castlora/releases).

The Android app asks only for the Internet permission, which it needs to import games from Chess.com.

## Privacy

- **No account and no Castlora server.** The developer receives no personal data.
- Your games, analysis and training data are stored **only on your device**: browser storage (IndexedDB) for the web app, app storage on Android.
- **No cookies, analytics, ads or tracking.**
- When you import from Chess.com, your device contacts `api.chess.com` directly with the username you entered (Chess.com also sees your IP address, as with any website). GitHub serves the website and the downloads.
- Back up with **Settings → Export**, and remove everything with **Settings → Delete all data**.

Read the full [privacy policy](https://william-lindberg.github.io/castlora/privacy.html).

## FAQ

**Is it really free?**
Yes. There's no subscription and there are no ads. Everything runs on your device, so there are no servers to pay for.

**Why is my accuracy different from Chess.com's?**
Castlora uses Stockfish 19 lite on your device, with its own settings and formula. Chess.com uses different ones. All evaluations and accuracy numbers are estimates.

**Where is my data?**
On your device only. It isn't synced. Use Settings → Export to move it to another device.

**Can I use it during a game?**
No. Castlora is for completed games only. Using analysis tools during a game breaks the fair play rules of Chess.com and other sites.

**Is Castlora open source?**
No. See below.

## Licence

Castlora is **free to use, but it is not open source**. The source code is not published, and this repository contains only the built website and the Android releases. You may use Castlora for personal, non-commercial purposes. You have **no permission to copy, modify, redistribute or rebrand** it, or to use it commercially, without written permission. Forking this repository on GitHub gives no additional rights. See [`LICENSE`](LICENSE) for the full Castlora License.

Third-party components keep their own licences. They are listed on the [open-source licences and notices](https://william-lindberg.github.io/castlora/notices.html) page. The **Stockfish** chess engine (`engine/stockfish-19-lite-single.js` and `.wasm`) is a separate, unmodified program under the **GNU GPL v3**, and your GPL rights for those files are not restricted. Its complete source code: [nmrugg/stockfish.js v19.0.1](https://github.com/nmrugg/stockfish.js/tree/v19.0.1) and [official-stockfish/Stockfish](https://github.com/official-stockfish/Stockfish). GPL text: [`engine/COPYING.txt`](engine/COPYING.txt).

Also see the [terms of use](https://william-lindberg.github.io/castlora/terms.html).

## Not affiliated

Castlora is not affiliated with Chess.com, Lichess or the Stockfish project.

## Contact

Open an [issue](https://github.com/William-Lindberg/castlora/issues) or contact [@William-Lindberg](https://github.com/William-Lindberg) on GitHub. Issues are public, so please don't include personal information.

---

© 2026 William Matthew Lindberg. All rights reserved.
