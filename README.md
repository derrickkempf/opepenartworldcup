# Opepen Art World Cup — minimal edition

One HTML file, no build step, no dependencies beyond the Firebase CDN script.
Open `index.html` (or host it anywhere static).

The single-file prototype is the base — its background grid, pixel-art
composition, and Firebase crowd voting are unchanged — with minimal versions
of the opepenwc features added:

- **90-minute matches in 90 seconds**: kickoff countdown, two 45s halves
  (1 second = 1 match minute), halftime, full-time hold; matches run
  back-to-back. Voting only while a match is live; most votes at FT advances
  (ties go to the higher seed).
- **Pages** (hash-routed, one file): Play, Teams & Kits (combined viewer:
  40 teams x home/away kits x 5 pitches), Bracket, Standings, Earn, Rules,
  Profile.
- **Match info** revealed at full time (votes + flavour stats).
- **Taste Points** (device-local): +25 per vote, +100 per correct pick,
  small bonuses on Earn.
- **Team names** from opepenwc's roster.

The demo clock anchor starts the tournament a few matches ago
(`const START` in the script) — set a fixed `Date.UTC(...)` timestamp there
for a real, shared event. Votes still use the same Firestore schema
(`matchups/{lo-hi}` with `a`/`b` counters), so existing data keeps working.
