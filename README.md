# The Opepen Art World Cup

### Your gut knows. Now prove it.

Forty artworks enter. One lifts the Cup. The bracket is decided by the fastest,
most honest reaction you have — the one you feel before you can explain it.

How long does it actually take you to know whether you love a piece? For most
people it's under three seconds. Then they spend ten minutes talking themselves
out of it. Every art ranking you've ever seen is built on those ten minutes —
filtered through critics, committees, algorithms, or raw click counts. None of
them measure the three seconds. **This does.**

---

## The premise

Two artworks appear. You pick the one that pulls you in. That's it — that's the
whole game, and it's harder than it sounds, because the clock is running and
your instinct is on the record.

- **Critic's choice:** months of deliberation.
- **Algorithm's choice:** whoever got the most clicks.
- **Your nervous system's choice:** ninety seconds.

Only one of those is honest. We built the tournament around it.

---

## How it works

**Every vote is a shot on goal.** You don't just register an opinion — you take
a shot, and *how you decide* determines where it lands.

- **Decide fast** and the shot finds the center of the net. Pure conviction.
- **Hesitate** and it drifts wide of the post. Doubt costs accuracy.
- **Keep changing your mind** and you'll eventually put it into your *own* net —
  more than two changes and it's an **own goal**, and your shot scores for the
  artwork you abandoned.

**Matches are 90 minutes played in 90 seconds** — a kickoff, two 45-second
halves (one second per match-minute), a halftime, and a full-time whistle,
running back to back. You can only shoot while the match is live. When the
whistle blows, the artwork the crowd reached for fastest goes through. Forty
become twenty, twenty become ten, and round by round, one is left holding the
Cup.

At full time the match opens up: goals, shots on target, own goals forced, and
the average decision time of the whole crowd — the anatomy of a collective gut
call.

---

## The kickoff

The Cup doesn't start on a schedule. It starts on a **quorum.**

The tournament stays on the bench until **80 people join.** The moment we hit
80, a **24-hour countdown** begins — and when it reaches zero, the whistle
blows and the first match goes live. No commissioner, no press conference. The
crowd decides when it's real, and then the crowd decides everything after.

Can't wait? The **demo** lets you play a match right now and feel the mechanic —
then help drag the counter toward 80. Share your code, bring people in, and earn
Taste Points for every soul you pull off the sidelines.

---

## What makes it different

| The old way | The Art World Cup |
|---|---|
| Paralysis | A 90-second clock that forces the honest answer your brain already has |
| Critic | You don't observe the result — you score it, miss it, shape it |
| Opinion | Evidence: exactly how fast and how confidently the world chose |
| Popularity | Conviction — not the most-clicked piece, the one people reached for first |

No names on the pitch, by the way — just numbers, **#41 through #80.** The work
speaks. You react. That's the only credential that counts here.

---

## Run it

It's **one HTML file.** No build, no framework, no install.

```
open index.html
```

Double-click it, or drop it on any static host. Everything — the artwork, the
pitch, the animation, the whole tournament engine — lives inside that single
file as code. The only things it reaches out for are the Geist font and (if you
choose to switch it on) Firebase for shared, live crowd voting.

## Make it live

To run a real, shared Cup where "80 people" means 80 *actual* people and votes
sync across every screen, connect Firebase and deploy the file. Full
step-by-step instructions — hosting, Firebase config, security rules, launch
control, and the owner tools — are in **[DEPLOY.md](./DEPLOY.md).**

A few things worth knowing:

- **Shared by default when connected.** Joins, the launch countdown, and every
  vote flow through Firebase (`matchups` and `meta` collections) so the crowd
  sees one truth. With no config, it runs fully offline as a personal demo.
- **Taste Points (TP)** are the game's currency of conviction — earned for
  voting, correct predictions, sharing, and daily check-ins. TP has no monetary
  value; it's a scoreboard for taste.
- **The advertising boards** ringing the pitch are yours to program. Only the
  owner can edit them (unlock with your passcode) — sell them, brand them, or
  leave them talking to themselves.

---

*A DEWD idea. Forty artworks. Ninety seconds. Your gut decides the champion.*
