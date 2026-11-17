# GitSquid

GitSquid is a personal build of [GitVolt](https://github.com/GitVoltApp/gitvolt), the Git client
by Francis Lavoie, with two things GitVolt doesn't ship:

- **An integrated terminal**: a terminal dock in each repository tab, with several terminals per
  tab.
- **Git Flow**: start and finish features, releases and hotfixes, including a finish that stops
  on a conflict and picks up again once it's resolved.

Everything else (the commit graph, diffs, worktrees, forge reviews, undo, and the rest) is
GitVolt's work. **If you don't need those two, use [GitVolt](https://github.com/GitVoltApp/gitvolt)
itself**: it's the original, and it moves fast.

GitSquid isn't affiliated with or endorsed by GitVolt or its author. Fixes that aren't specific to
GitSquid go upstream to GitVolt.

## Download

From the [latest release](../../releases/latest), which has every platform's package:

- **macOS 12 or later:** `GitSquid_<version>_aarch64.dmg` (Apple Silicon) or
  `GitSquid_<version>_x64.dmg` (Intel). Signed with a Developer ID and notarized: open it and
  drag GitSquid to Applications. It updates itself.
- **Windows 10 and 11 (x64):** `GitSquid_<version>_x64-setup.exe` (installs for you, no
  administrator rights) or `GitSquid_<version>_x64.msi` (installs for all users). They aren't
  code-signed yet, so SmartScreen warns the first time: **More info** › **Run anyway**. The
  integrated terminal isn't available on Windows yet.
- **Linux (x64):**
  - Debian and Ubuntu (24.04 or later): `sudo apt install ./GitSquid_<version>_amd64.deb`
  - Fedora 40 or later: `sudo dnf install ./GitSquid-<version>-1.x86_64.rpm`
  - Arch Linux: `sudo pacman -U ./GitSquid-<version>-1-x86_64.pkg.tar.zst` (here the version is
    written without its dash, e.g. `1.6.2sq.24`)

On Windows and Linux, the app tells you when there's a new version; install it from here.

Each release lists the SHA-256 of its packages in `SHA256SUMS`. A version reads
`<GitVolt version>-sq.<n>`: the GitVolt release it's based on, then GitSquid's build number.
macOS builds come out more often than the others: a release marked *Pre-release* has the macOS
packages only so far. Twice a week the newest release gets its Windows and Linux packages and
becomes the latest release.

GitSquid keeps its settings, install folder and package names apart from GitVolt's, so the two
can be installed side by side, and removing one leaves the other alone.

## Feedback

Open an [issue](../../issues) here. Please don't report GitSquid problems to GitVolt: if one turns
out to be GitVolt's own, it's reproduced in GitVolt and reported there.

## License

[MIT](LICENSE). GitSquid is based on GitVolt, Copyright (c) 2026 Francis Lavoie, under the MIT
license; the app credits it under **About**, and its bundle carries the licenses and third-party
notices of everything it ships (on macOS in `GitSquid.app/Contents/Resources/licenses`, on
Windows in the install folder's `licenses`, on Linux in `/usr/share/doc/gitsquid`).
