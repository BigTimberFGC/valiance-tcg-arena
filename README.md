# Valiance TCG for TCG Arena

This folder is a TCG Arena custom-game package, not a replacement game app.
It converts the included rulebook's tabletop structure into Arena's board,
deck-building, counters, and turn handling.

## Included rules support

- 100 starting health, 5-page opening plan, 40-60 page spellbooks, and a
  three-copy limit.
- Dedicated Play Area, Familiar Zone, Construct Zone, Spellbook, and public
  Memory.
- Aether and Spell Power controls for each player. Aether is capped at 10,
  initializes the final player at 1, and charges automatically on that
  player's recovery turn. Spell Power clears when a new turn begins.
- Rulebook terminology and the Recovery → Planning → Action → End sequence in
  Arena's in-game help.
- One-click cleanup from the Play Area into Memory.

TCG Arena is a tabletop simulator, so targets, skill text, priority, combat
comparisons, and Familiar uniqueness remain visible player actions. This is
intentional: Arena does not implement individual card effects automatically.

## Load from GitHub

No local server is required. This package is staged for the public repository
`BigTimberFGC/valiance-tcg-arena`. Once published, load it in TCG Arena here:

`https://tcg-arena.fr/load/aHR0cHMlM0ElMkYlMkZyYXcuZ2l0aHVidXNlcmNvbnRlbnQuY29tJTJGQmlnVGltYmVyRkdDJTJGdmFsaWFuY2UtdGNnLWFyZW5hJTJGbWFpbiUyRkdhbWUuanNvbg==`

That loader reads the public
`https://raw.githubusercontent.com/BigTimberFGC/valiance-tcg-arena/main/Game.json`
file, which in turn references the card catalogue and mat assets directly from
GitHub. The catalogue includes all 115 card faces from the supplied Untap card
list, linked as direct Imgur images, plus fourteen project demo Pages. The
imported entries use generic **Page** metadata because the CSV supplies titles
and artwork—not structured cost, power, type, or rules text. Read each printed
card face as the authority until richer card data is available.
