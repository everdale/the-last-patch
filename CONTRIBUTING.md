# Contributing to The Last Patch — the production system

This file answers Håkan's point 8 directly: *what does the repo need so that anyone — me, you, a future and different AI model — can keep adding high-quality, **diverse** content without the worlds blurring together, the voices collapsing, or the puzzles going one-directional?*

The answer is an **assembly line**: a fixed sequence of gates, each backed by a doctrine doc, that a new world must pass before it's canon. The gates are deliberately constraining. Constraints are what keep a single (especially AI) author from regressing to one house style. **Diversity is enforced, not hoped for.**

## The north-star docs (read before contributing)

| Doc | Owns the question |
|---|---|
| [docs/design.md](docs/design.md) | What is this game and what is it *for*? (completion & memory, not retention) |
| [docs/the-mechanic.md](docs/the-mechanic.md) | The USP: inventory-as-debugger (Lens + Spanner). Why it's a game, not a VN. |
| [docs/humor-doctrine.md](docs/humor-doctrine.md) | How comedy is built (bits not premises; enacted not read; the kill-rate). |
| [docs/puzzle-design.md](docs/puzzle-design.md) | The 8 tiers + the distribution rule that prevents monotony. |
| [docs/voice-bible.md](docs/voice-bible.md) | Voice Cards + the Strip-Names test that prevents same-voice collapse. |
| [docs/world-traversal.md](docs/world-traversal.md) | Discovery-long / return-instant. The map contracts. |
| [docs/tickets.md](docs/tickets.md) | The backlog. Every world is a ticket framed as a *bit*. |

## The assembly line — building one new world

Copy [vignettes/_TEMPLATE.md](vignettes/_TEMPLATE.md) to `vignettes/<bug-id>-<name>/script.md` and pass these gates **in order**. Each gate has a hard rejection condition.

**Gate 0 — The Ticket (the bit).**
State the world as one line in the bug tracker, and name the central character's **want → plan → backfire**. *Reject if you can only name a quirk.* ("Monster has stage fright" = quirk = reject. "Monster ordered a mirror-maze to feel surrounded, saw himself, became a narcissist" = bit = pass.)

**Gate 1 — The One Absurdity.**
Write the single broken rule. Then write three ways the world takes it *dead seriously* (economy, religion, infrastructure, manners). *Reject if there's a second, unrelated absurdity* — one per land (humor-doctrine §4).

**Gate 2 — Voice Cards.**
Fill a six-axis Voice Card (voice-bible) for every speaking character, under the world's house-style. Then run the **Engine-Collision check**: no two characters share a comedic engine. *Reject on collision.*

**Gate 3 — The Puzzle Histogram.**
Design the puzzles and tag each by tier (puzzle-design). *Reject unless: ≥4 of 8 tiers present; no 3 consecutive same-tier; opens tier 1–2; story-gate ≤ tier 5; ≤1 tier-8 gag; the new verb is taught easy before it's gated.*

**Gate 4 — Fairness pass.**
Every non-obvious puzzle has: a soft hint in the world, a "stop digging" signal, and a slot in the escalating hint button. *Reject any puzzle solvable only by moon-logic.*

**Gate 5 — The Verb & the Warp.**
Name the debugger verb this world teaches and the Warp Node / shortcut it drops on completion (world-traversal). *Reject if revisiting requires >2 screens of re-traversal.*

**Gate 6 — The Mercy & the Mastery (1+4 law).**
A generous story-clear bar (~minutes, diegetic mercy on failure) **and** optional mastery tiers. *Reject if failure produces a wall instead of content.*

**Gate 7 — The Bill (the thesis).**
Every fix opens a second ticket. Write the `BUG-xxx OPENED` that your fix causes, and how it pays out later (a letter, an NPC at Patched Anonymous, a return contract). *Reject a fix with no cost* — the whole game is about the cost.

**Gate 8 — The Red Pen.**
Draft long, then cut. End the script with a self-flagged **kill list** (lines you suspect; lines you'd defend). Run the **Strip-Names test** on three lines. *Reject if any line falls flat on a second read or any voice is unassignable.*

## The kill-rate principle

First-draft comedy — human or AI — regresses to "wacky." The funny lives in the third detail (gel pen, anxious stars). **Volume is raw material, never product.** Expect to cut half. A contribution that wasn't cut down probably wasn't punched up. The gate that matters most is the cheapest one: it's all paper until the script is funny.

## Repo layout

```
docs/            the doctrine (north stars above)
vignettes/       one folder per world; script.md is the source of truth
  _TEMPLATE.md   copy this to start a world
  bug-031-penultima/   first scripted world (the dialogue gate)
demo/            playable prototypes (open the .html files directly)
  index.html         BUG-031 narrative vignette (both paths + letters)
  puzzle-proto.html  BUG-072 the Bard's Clock — the inventory-as-debugger mechanic
```

## If you are an AI contributor (you probably are)

Your specific failure mode is **sameness**: one wit, one rhythm, one joke shape across every character and world. The Voice Cards, the Engine-Collision check, the Strip-Names test, and the puzzle distribution rule exist precisely to fight *you*. Treat them as non-negotiable. When in doubt, make two characters **more different than feels natural** — the natural pull is toward collapse. And never explain a joke in the text; if it needs a second read, it's dead (humor-doctrine §7).
