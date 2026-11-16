# GitSquid

GitSquid is a personal build of [GitVolt](https://github.com/GitVoltApp/gitvolt), the Git client
by Francis Lavoie, with two things GitVolt doesn't ship:

- **An integrated terminal**: a terminal dock in each repository tab, with several terminals per
  tab.
- **Git Flow**: start and finish features, releases and hotfixes, including a finish that stops
  on a conflict and picks up again once it's resolved.

Everything else (the commit graph, diffs, worktrees, forge reviews, undo, and the rest) is
GitVolt's work. **If you don't need those two, use [GitVolt](https://github.com/GitVoltApp/gitvolt)
itself**: it's the original, it moves fast, and it runs on Linux and Windows too.

GitSquid isn't affiliated with or endorsed by GitVolt or its author. Fixes that aren't specific to
GitSquid go upstream to GitVolt.

## Download

macOS 12 or later. From [Releases](../../releases):

- Apple Silicon: `GitSquid_<version>_aarch64.dmg`
- Intel: `GitSquid_<version>_x64.dmg`

Each release lists the SHA-256 of both in `SHA256SUMS`. A version reads
`<GitVolt version>-sq.<n>`: the GitVolt release it's based on, then GitSquid's build number.

GitSquid keeps its settings apart from GitVolt's, so the two can be installed side by side.

## Feedback

Open an [issue](../../issues) here. Please don't report GitSquid problems to GitVolt: if one turns
out to be GitVolt's own, it's reproduced in GitVolt and reported there.

## License

[MIT](LICENSE). GitSquid is based on GitVolt, Copyright (c) 2026 Francis Lavoie, under the MIT
license; the app credits it under **About**, and its bundle carries the licenses and third-party
notices of everything it ships (`GitSquid.app/Contents/Resources/licenses`).
