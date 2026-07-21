# Contributing

Thanks for helping! Contributions to a color theme are mostly small CSS
tweaks, palette corrections, and compatibility reports.

## Ways to contribute

- **Bug reports**: use the bug report template and attach a screenshot showing
  the problem.
- **Palette corrections**: keep changes inside the official Solarized palette
  where possible, and mention which palette role a color maps to.
- **Code and docs**: pull requests welcome.

## Workflow

1. Branch from `main` using `feat/`, `fix/`, or `docs/` prefixes.
2. Keep commits in [Conventional Commits](https://www.conventionalcommits.org)
   style (`feat:`, `fix:`, `docs:`, `chore:`).
3. Fill in the pull request template. Visual changes require before and after
   screenshots in the same PR.
4. CI validates `manifest.json` and the theme files on every push and pull
   request, so keep it green.

## Testing your changes

Run ULauncher with the local copy of the theme before opening a PR:

```bash
ulauncher --dev --no-window-theme --theme-path "$PWD"
```

Check both the default result list and a query with matched text highlighting.

## Releases

The release workflow attaches an installable zip to GitHub Releases for every
`v*` tag.
