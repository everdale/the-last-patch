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
- **"Every fix opens two tickets"** — kept, but reframed from a thesis into a **toy** (the WONTFIX cascade, [ending-candidates.md](ending-candidates.md)). **The Update** and **Patched Anonymous** are now *optional* (the end-game antagonist becomes your own compulsion to fix). The ending is a diegetic genre-nod, not a fourth-wall meta-ending — much lower-risk. Open: framing (i) "had WONTFIX all along" vs (ii) "earn it in the chaos". Paper gate: write 3–4 cascade chains and check they're funny cold.
- **The gamedev theme itself.** Survives a re-theme (the structure is "fixer enters broken worlds"). Held option.

## ⚪ Example only (illustration, never a spec)

- **The Bard's Clock** ([demo/puzzle-proto.html](../demo/puzzle-proto.html)). Built to prove a mechanic *can* be a game, not because the clock puzzle should exist. The clock was Håkan's throwaway example; I over-delivered on it. The keepers are the *principles* (a hint can hide in dialogue; a "stop digging" signal must bound the search) — not the puzzle.
- Any specific puzzle, line, or character detail in the scripts: tone samples, not commitments.

## ❓ Open questions (need a decision before they stop blocking downstream work)

1. **Spine weight.** Light adventure (powers are comedic conveniences, story carries you) vs. fuller metroidvania (powers gate the map). This decides a *lot*. Håkan is wary of the metroidvania (point 3).
2. **Cross-world inventory scope.** If items/verbs travel between worlds, how do we avoid the Day-of-the-Tentacle combinatorial-frustration problem? (See [the toolbox](../CONTRIBUTING.md#scope--gating-managing-the-move-space).)
3. **Theme.** Keep gamedev, or hold it as a swappable skin?
4. **Demo fidelity / art.** Current stance: low-fi, text-forward prototypes with an *inferred* (non-animated) protagonist and placeholder visuals — prove logic/dialogue/mechanics, commit no character art until the foundation is set. (Håkan, point 5 — provisionally agreed.)

## 🔬 Research

- ✅ **Competitive teardown** — done: [teardown-pointandclick.md](teardown-pointandclick.md). Differential analysis (Escape from Monkey Island as the controlled probe) of what sinks vs. carries genre entries, and the deliberate blend that makes us novel rather than a clone. **Key finding that changes a decision:** Gilbert's meta-endings reliably *divide* fans because they *sever* rather than *recontextualise* — and our candidate ending is meta and thesis-heavy, so the "recontextualise test" is now a hard rule and an early-prototype priority.
- ⏳ **Still worth doing:** a hands-on pacing pass once a real vignette is built (analysis can't settle whether the inspect/patch verb stays fun across 5+ worlds — the Monkey Kombat risk applies to any verb).
