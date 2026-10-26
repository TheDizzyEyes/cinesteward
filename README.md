# CineSteward

[![Latest version](https://img.shields.io/github/v/release/TheDizzyEyes/cinesteward?label=latest%20version)](https://github.com/TheDizzyEyes/cinesteward/releases/latest)

CineSteward keeps track of the shows and movies you watch, on Windows, macOS and Linux. Tick off episodes as you go, see what's next and what's coming, and share it all with your friends.

## Install

CineSteward runs on 64-bit Windows 10 and 11. You don't need administrator rights, and nothing else has to be installed first.

**The setup file:** download [CineSteward-Setup.exe](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-Setup.exe) and double-click it. Choose where it goes (or keep `Documents\CineSteward`) and click **Install**.
CineSteward isn't code-signed yet, so Windows may first say **Windows protected your PC**: choose **More info → Run anyway**.

**Or with one line in PowerShell**, which skips that warning:

```powershell
irm https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/install.ps1 | iex
```

After that, CineSteward keeps itself up to date: when a new version is out, it offers it in the app. To remove it, go to **Settings → Apps → Installed apps** in Windows. Your library stays on your PC unless you choose to delete it too.

**On a Mac**, download [CineSteward-mac-arm64.dmg](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-mac-arm64.dmg) for Apple silicon (M1 and later) or [CineSteward-mac-x64.dmg](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-mac-x64.dmg) for an Intel processor, open it and drag CineSteward onto **Applications**. macOS stops it once because it isn't notarised by Apple yet: choose **System Settings → Privacy & Security → Open Anyway**. CineSteward needs macOS 15 or later.

**On Linux**, download [CineSteward-linux-x64.AppImage](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-linux-x64.AppImage) (Intel and AMD) or [CineSteward-linux-arm64.AppImage](https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/CineSteward-linux-arm64.AppImage) (ARM), allow it to run once in its Properties, and double-click it. The distributions it runs on are in the [changelog](https://github.com/TheDizzyEyes/cinesteward/releases) of 1.37.0, and SteamOS since 1.40.0.

**Or, on a Mac or on Linux, paste this into Terminal**, which also puts CineSteward in your applications menu on Linux and skips the macOS warning:

```bash
curl -fsSL https://github.com/TheDizzyEyes/cinesteward/releases/latest/download/install.sh | sh
```

After that, CineSteward offers new versions in the app and installs them itself.

**On a Steam Deck**, install it in Desktop Mode with the Terminal line above (in Konsole), then right-click CineSteward in the application launcher and choose **Add to Steam** to start it from Game Mode too. The controller works it, and tapping a box to type in brings up Steam's keyboard.

## Main features

- **Shows and movies in one place:** what you're watching, have finished, put on hold, dropped or plan to watch, plus lists of your own.
- **Episodes:** +1 episode in one click, tick any episode or a whole season, and rewatches with their own progress.
- **Up Next and Calendar:** the next episode of everything you're watching, and a month of new episodes and releases.
- **Notifications:** new episodes, new seasons, and titles on your watchlist that start streaming on your services.
- **Search and discovery:** search with filters, what's trending, "Because you liked…", and Pick for me when you can't decide.
- **Details:** trailers, cast and crew, where it streams, franchises, ratings in half stars, tags and your own review.
- **Profile:** your top 4 favourites, your stats and badges, charts, a watch calendar with streaks, your year in review, and pictures to share.
- **Friends:** add friends with a friend code and see what they're watching, react, recommend titles, compare your tastes, comment, and watch shows together with episodes ticked off for both of you. A spoiler shield hides what friends say about episodes you haven't seen yet.
- **Bring your history:** import what you watched and when, your ratings, reviews and watchlist from Letterboxd, IMDb, Trakt, TV Time, Netflix, Showcase or Simkl.
- **Backups:** save one yourself, or let CineSteward save a dated backup every day, week or month in a folder you choose, such as one OneDrive or Google Drive keeps in step.
- **Your way:** light and dark themes, accent colours, larger text and higher contrast.

## Latest version

The newest version, and what changed in it, is always on the [releases page](https://github.com/TheDizzyEyes/cinesteward/releases/latest). Every change is also listed in the app under **Settings → App**.

## Questions

In the app, **CineSteward** is first among your friends: write to it to report a problem, suggest an idea or ask a question, and the answer comes there. You can also ask on Discord: <https://discord.gg/theofficialroundtable>

---

Show and movie data and images come from [TMDB](https://www.themoviedb.org/). CineSteward uses the TMDB API but is not endorsed or certified by TMDB.
