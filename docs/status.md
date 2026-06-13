# Commitment Status — what's decided vs. what we're auditioning

The point of this file is honesty about *commitment level*. The previous doc pass wrote a lot of speculative ideas as if they were settled. They aren't. Nothing below is canon until Håkan promotes it here. **This is a proposed classification — correct it freely; that's its job.**

Read every other doc through this lens: if an idea is tagged **candidate** or **example** here, treat its appearance elsewhere as "one option we're exploring," not "the design."

---

## ✅ Decided (load-bearing; would take a real argument to move)

- **The fantasy:** you're a fixer who steps *inside* broken games and repairs them from within. (The "Debugger" name is itself only a candidate.)
- **The bar for comedy:** character + situation, not quirks or one-liners. Jokes are *enacted*, not read. (See [humor-doctrine.md](humor-doctrine.md) — this aligns with Håkan's stated taste and is the closest thing to settled.)
- **The KPI:** completion and memory, not retention. Finished and quoted, not endless.
- **It must be a *game*:** real interactivity and puzzles, not a visual novel with choices.
- **Voices stay distinct; worlds feel distinct.** No house-wit collapse, no copy-paste world shape.

## 🟡 Candidate (promising, actively auditioning — NOT committed)

- **Inventory-as-debugger (Lens + Spanner).** My current best proposal for the USP. Strong, unproven. Could change form entirely.
- **The earned-verbs / metroidvania spine** (Save Scum, Noclip, Pause, Cutscene Skip, Patch). Interesting *and* scary (Håkan, point 3). Held, not adopted. The spine's *weight* is an open question below.
- **The specific worlds** — Penultima and the genre-land roster in [tickets.md](tickets.md) — are a candidate menu and a tone test, **not a committed lineup.** Expect cuts.
- **"Every fix opens two tickets"** as the thesis; **The Update** as villain; **Patched Anonymous** as the thesis room. Thematically rich, still optional.
- **The gamedev theme itself.** Survives a re-theme (the structure is "fixer enters broken worlds"). Held option.

## ⚪ Example only (illustration, never a spec)

- **The Bard's Clock** ([demo/puzzle-proto.html](../demo/puzzle-proto.html)). Built to prove a mechanic *can* be a game, not because the clock puzzle should exist. The clock was Håkan's throwaway example; I over-delivered on it. The keepers are the *principles* (a hint can hide in dialogue; a "stop digging" signal must bound the search) — not the puzzle.
- Any specific puzzle, line, or character detail in the scripts: tone samples, not commitments.

## ❓ Open questions (need a decision before they stop blocking downstream work)

1. **Spine weight.** Light adventure (powers are comedic conveniences, story carries you) vs. fuller metroidvania (powers gate the map). This decides a *lot*. Håkan is wary of the metroidvania (point 3).
2. **Cross-world inventory scope.** If items/verbs travel between worlds, how do we avoid the Day-of-the-Tentacle combinatorial-frustration problem? (See [the toolbox](../CONTRIBUTING.md#scope--gating-managing-the-move-space).)
3. **Theme.** Keep gamedev, or hold it as a swappable skin?
4. **Demo fidelity / art.** Current stance: low-fi, text-forward prototypes with an *inferred* (non-animated) protagonist and placeholder visuals — prove logic/dialogue/mechanics, commit no character art until the foundation is set. (Håkan, point 5 — provisionally agreed.)

## 🔬 Research to do (Håkan, point 4)

- **Competitive teardown** of point-and-click balancing — how good ones (and instructive bad ones) pace puzzles vs. dialogue vs. exploration, gate the move-space, and manage inventory scope. Candidates to study: Monkey Island 1–2, Day of the Tentacle, Grim Fandango, Edna & Harvey, Thimbleweed Park, Return of the Obra Dinn (for deduction), and a deliberate bad/uneven example or two. Not started; do before locking puzzle/gating doctrine.
