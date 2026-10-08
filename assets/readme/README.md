# README artwork

The repository-root README uses local SVGs with outlined Outfit lettering. The
original `assets/branding/logo.svg` is preserved; the hero embeds its existing
image without changing the mark. PNG exports of the hero and overview replace
the previous files at the same paths.

The palette is charcoal `#181818`, warm neutral `#D5D8C5`, green `#18B880`,
orange `#F9771D`, and muted red `#CE6969`. Banners share a 1200 × 104 canvas;
the hero is 1200 × 496. PNGs are exported at twice the SVG dimensions.

To regenerate from the repository root:

```sh
python -m pip install -r assets/readme/source/requirements.txt
python assets/readme/source/generate.py
```

The script reads only the checked-in logo and font. It does not download assets
or require application dependencies. SVG text is converted to paths, so the
README does not depend on browser fonts, CSS, scripts, or remote image services.

Outfit is distributed under the SIL Open Font License. Its font file and license
are included in `assets/branding/fonts/`.
