Emberhold — Living World Dungeon Crawler (full source export)
Exported: 2026-11-19T15:33:51.686Z

Contents:
  main.pjs   - perchance generator code (lists / config)
  index.html - game HTML: full document (UTF-8 BOM + doctype/<head> wrapper,
               then the generator body). Pasting it into a Perchance HTML
               panel is safe: doctype/html/head tokens are ignored in body
               context and the BOM is invisible.
  src/       - all game modules, data, sprites, shots — including
               tauri-bridge.js and update-check.js, which no-op outside the
               Tauri desktop shell
  assets/    - bundled title logo (offline title screen)

How to use:
  - This is a perchance.org generator. To restore: create a new generator,
    replace its main.pjs + index.html with these files, and upload src/ files
    to the same relative paths (src/...).
  - Or host index.html + src/ statically for the non-perchance parts, but full
    game requires the Perchance engine (main.pjs evaluation, plugins).
  - The Tauri desktop shell (github.com/Devanand-PA/emberhold-tauri) serves
    this tree as-is: its sync is a plain copy, no overlay or patch step.

File count: 83
