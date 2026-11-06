# Mirror Match (CHEM 3B stereochemistry)

Study game for CHEM 3B stereochemistry: textbook Sections 3.2 (cis–trans), 5.5 (chirality), 8.2–8.3 (D and L sugars, Fischer projections) and 10.1 (L-amino acids). Live at https://itsdrdan.github.io/stereochemistry/ once GitHub Pages is on.

- `index.html`: the whole game (standalone; no build step). Built on the Enzyme Engine game shell. Loads the brand kit (`games/brand/itsdrdan.css`, `icons.js`, `embed.js`), `games/track.js` for anonymous stats (game id `stereochemistry`), and `textbook/js/fbx.js`, which draws every structure (the same renderer the textbook and Final Boss use) and runs Exam Practice from `textbook/bank/chirality.json` and `isomers.json`.
- 5 main options → 13 topics: Chiral Carbons (key terms, spot the chiral carbon, count chiral carbons, 2ⁿ stereoisomers), Isomer Relationships (enantiomers/diastereomers/identical on wedge-and-dash drawings; constitutional vs identical), Cis & Trans (alkenes, rings), Fischer & D/L (sugars, amino acids, compare two Fischer projections, pick the enantiomer), Health & Clinic (chiral drugs). Plus Skill Check Prep (10 questions → study plan) and Exam Practice.
- Every molecule is generated in code and the answer is computed from the structure: chiral carbons by comparing all four groups, relationships by comparing every chiral carbon (drawings flipped left to right count as reversed). 400 generated relationship pairs were checked against RDKit with zero disagreements (Nov 5, 2026).
- `ASSETS.md`: the art list (mascot Mira, logo, badges). Stand-ins show until the files exist.
- Links: `?topic=find,relate` opens topics directly; `?mode=exam` opens Exam Practice.

Game design and chemistry by ItsDrDan. Code written with AI assistance (Claude) and checked by the author. © ItsDrDan, all rights reserved; free to play, reuse by permission only (see LICENSE).
