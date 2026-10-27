# CineSteward

[![Latest version](https://img.shields.io/github/v/release/TheDizzyEyes/cinesteward?label=latest%20version)](https://github.com/TheDizzyEyes/cinesteward/releases/latest)

CineSteward keeps track of the shows and movies you watch, on Windows, macOS and Linux. Tick off episodes as you go, see what's next and what's coming, and share it all with your friends.

**Jump to:** [Install](#install) · [Main features](#main-features) · [Latest version](#latest-version) · [Questions](#questions)

## Install

Pick the download for your computer. Each one is the latest version, and CineSteward keeps itself up to date after that.

| Your computer | Download | Needs |
| --- | --- | --- |
| 🪟 **Windows** | [CineSteward-Setup.exe](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-Setup.exe) | 64-bit Windows 10 or 11 |
| 🍎 **Mac with Apple silicon** (M1 and later) | [CineSteward-mac-arm64.dmg](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-mac-arm64.dmg) | macOS 15 Sequoia or later |
| 🍎 **Mac with an Intel processor** | [CineSteward-mac-x64.dmg](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-mac-x64.dmg) | macOS 15 Sequoia or later |
| 🐧 **Linux** on Intel or AMD | [CineSteward-linux-x64.AppImage](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-linux-x64.AppImage) | 64-bit, with a desktop such as GNOME, KDE Plasma, Cinnamon or Xfce |
| 🐧 **Linux** on ARM | [CineSteward-linux-arm64.AppImage](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-linux-arm64.AppImage) | the same |
| 🎮 **Steam Deck** | the Terminal line below, in Desktop Mode | SteamOS 3 |

You don't need administrator rights, and nothing else has to be installed first.

### 🪟 Windows

1. Download [CineSteward-Setup.exe](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-Setup.exe) and double-click it.
2. Choose where CineSteward goes (or keep `Documents\CineSteward`) and click **Install**.
3. CineSteward isn't code-signed yet, so Windows may first say **Windows protected your PC**. Choose **More info**, then **Run anyway**.

Or install it with one line in PowerShell, which skips that warning:

```powershell
irm https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/install.ps1 | iex
```

To remove it, go to **Settings → Apps → Installed apps** in Windows. Your library stays on your PC unless you choose to delete it too.

### 🍎 macOS

1. Download the disk image for your Mac: [Apple silicon](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-mac-arm64.dmg) (M1 and later) or [Intel](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-mac-x64.dmg). Not sure which? Choose **Apple menu → About This Mac**: it says **Chip Apple M…** or **Processor Intel**.
2. Open it and drag CineSteward onto **Applications**.
3. CineSteward isn't notarised by Apple yet, so macOS stops it the first time. Choose **System Settings → Privacy & Security**, scroll down, and click **Open Anyway** next to CineSteward.

Or paste this into Terminal, which picks the right version for your Mac and skips that step:

```bash
curl -fsSL https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/install.sh | sh
```

To remove it, drag CineSteward from **Applications** to the Bin. Your library stays in `~/Library/Application Support/CineSteward`.

### 🐧 Linux

1. Download the AppImage: [Intel or AMD](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-linux-x64.AppImage) (x64) or [ARM](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-linux-arm64.AppImage) (arm64).
2. Right-click it, open **Properties**, and allow it to run as a program (or run `chmod +x CineSteward-linux-*.AppImage`).
3. Double-click it.

Or paste this into a terminal, which also puts CineSteward in your applications menu:

```bash
curl -fsSL https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/install.sh | sh
```

To remove what that line installed, run it again with `--uninstall` at the end: `... | sh -s -- --uninstall`. An AppImage you simply delete. Your library stays in `~/.local/share/CineSteward`.

<details>
<summary>The Linux distributions CineSteward runs on</summary>

- Ubuntu 22.04, 24.04 and 26.04
- Debian 13
- Fedora 43 and 44
- Linux Mint 21 and 22, Pop!_OS 22.04 and 24.04, Zorin OS 17, and elementary OS 7 and 8, which are built on Ubuntu
- openSUSE Leap 16.0, and SUSE Linux Enterprise 15.7 and 16.0
- Red Hat Enterprise Linux 8, 9 and 10, AlmaLinux and Rocky Linux, and CentOS Stream 9 and 10
- SteamOS 3, on a Steam Deck

Others with glibc 2.27 or later, like Arch Linux and Manjaro, usually work too. Alpine Linux doesn't, as it has no glibc.

</details>

### 🎮 Steam Deck and controllers

1. On your Steam Deck, switch to **Desktop Mode**, open **Konsole** and paste the Terminal line from the Linux section above.
2. Right-click CineSteward in the application launcher and choose **Add to Steam**.
3. Back in Game Mode, start it from your library. The controller works it: the D-pad or left stick moves, **A** opens, **B** goes back, **X** opens a title's menu, the shoulder buttons change page and the right stick scrolls. Tapping a box to type in brings up Steam's keyboard.

On Windows, a controller works the same way when Steam starts CineSteward: add it to Steam with **Games → Add a Non-Steam Game to My Library** and start it from there, in Big Picture too.

### ✨ After installing

- **Sign in** under **Settings → Account** to get movie and show info and to add friends. Creating an account may ask for an invite code: ask the friend who told you about CineSteward.
- **Bring what you watched** from Letterboxd, IMDb, Trakt, TV Time, Netflix, Showcase, Simkl or a spreadsheet under **Settings → Library → Import from another app**.
- **Updates come by themselves:** when a new version is out, CineSteward says so and **Update now** installs it, on Windows, on a Mac and on Linux.

## Main features

- **Shows and movies in one place:** what you're watching, have finished, put on hold, dropped or plan to watch, plus lists of your own.
- **Episodes:** +1 episode in one click, tick any episode or a whole season, rate episodes, and rewatches with their own progress.
- **Up Next and Calendar:** the next episode of everything you're watching, also from the Windows taskbar, and a calendar of new episodes and releases you can save to Outlook, Google or Apple Calendar.
- **Where to watch:** the services that have a title in your country, yours first, and in which other countries it streams. **Your watchlist abroad** shows which of your watchlist your services only have elsewhere.
- **Notifications:** new episodes, new seasons, titles on your watchlist that start streaming on your services, and new work by the actors and directors you follow, with quiet hours for the night.
- **Search and discovery:** search with filters, what's trending, "Because you liked…", more like this, and Pick for me when you can't decide.
- **Details:** trailers, cast and crew, franchises, ratings out of 10, tags and your own review.
- **Profile:** your top 5, your stats and badges, charts (how you rate against TMDB, too), a watch calendar with streaks, your year in review set against the year before, and pictures to share.
- **Friends:** add friends with a friend code or an invite link and see what they're watching, react, recommend titles, compare your tastes, comment, and watch shows together with episodes ticked off for both of you. **Our list** keeps a watchlist with a friend, and you both vote 👍 or 👎. A spoiler shield hides what friends say about episodes you haven't seen yet.
- **Your library on all your computers:** switch it on and it stays the same on each of them.
- **Connected to what you use:** your watchlist and ratings mirrored to your TMDB account (both ways) and to Trakt, and what you play on your own Plex or Jellyfin server ticked off by itself.
- **Bring your history, and take it with you:** import from Letterboxd, IMDb, Trakt, TV Time, Netflix, Showcase, Simkl or a spreadsheet; export as a spreadsheet or for Letterboxd.
- **Backups:** save one yourself, or let CineSteward save a dated backup every day, week or month in a folder you choose, such as one OneDrive or Google Drive keeps in step.
- **Your way:** nine themes, accent colours (or your own), poster sizes, text from 80% to 200%, higher contrast, and the keyboard, a touchscreen or a controller.

## Latest version

The newest version, and what changed in it, is always on the [releases page](https://github.com/TheDizzyEyes/cinesteward/releases/latest). Every change is also listed in the app under **Settings → App**, sorted into what was added, changed and fixed.

## Questions

In the app, **CineSteward** is first among your friends: write to it to report a problem, suggest an idea or ask a question, and the answer comes there. You can also ask on Discord: <https://discord.gg/theofficialroundtable>

---

Show and movie data and images come from [TMDB](https://www.themoviedb.org/). Streaming availability comes from JustWatch, through TMDB. CineSteward uses the TMDB API but is not endorsed or certified by TMDB.
