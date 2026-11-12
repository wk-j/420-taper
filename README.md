# 420 Taper

A monospaced coding font: Share Tech Mono (via the Nerd Fonts patch, "Shure Tech Mono Nerd Font Mono")
whose stems narrow toward their free ends, plus an Italic that is the same tapered design slanted 10°.
Nerd Font icons, box drawing and Powerline separators stay square and upright. Latin only (no Thai).

## Build

Needs [uv](https://docs.astral.sh/uv/) (installs Python 3.11+ and fontTools from the script's inline metadata).

```sh
uv run build.py 420-taper.toml
```

Output: `dist/420Taper/420Taper-Regular.ttf` and `dist/420Taper/420Taper-Italic.ttf`.
Install by copying them into `~/Library/Fonts`, then pick **420 Taper** in your editor or terminal.

Tune the look in `420-taper.toml`: `taper.amount` (0.35 subtle, 0.5 default, 0.65 near-pointed),
`taper.length`, and `oblique.angle`.

## License

SIL Open Font License 1.1, see `OFL.txt`.
Copyright (c) 2012, Carrois Type Design, Ralph du Carrois, with Reserved Font Name 'Share'.
Nerd Fonts patch: Ryan L McIntyre (OFL). Modifications for 420 Taper are released under the same license.

- The family name must not contain "Share" (Reserved Font Name).
- Keep `OFL.txt` and the copyright notice with any copy of the fonts.
- The fonts may be bundled with software, but not sold on their own.

## Download

GitHub Actions builds the fonts on every push to `main` and on pull requests.
Download them from the run's **Artifacts** section (`420Taper`).
Push a tag such as `v1.0.0` to publish a Release with `420Taper.zip` and the `.ttf` files attached:

```sh
git tag v1.0.0 && git push origin v1.0.0
```
