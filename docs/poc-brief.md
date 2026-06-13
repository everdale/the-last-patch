# POC Brief — the next proof-of-concept

> Goal of the POC: prove the **core loop** of The Last Patch as one small, playable, low-fi slice — integrating what the two earlier demos showed separately (good dialogue/characters in [demo/index.html](../demo/index.html); a real inspect/patch puzzle in [demo/puzzle-proto.html](../demo/puzzle-proto.html)) into a single coherent vignette that actually feels like the game.

## Read first (the cold-start reading list)
[status.md](status.md) (what's decided vs candidate) → [the-mechanic.md](the-mechanic.md) → [humor-doctrine.md](humor-doctrine.md) → [puzzle-design.md](puzzle-design.md) → [the-antagonist.md](the-antagonist.md) → [ending-candidates.md](ending-candidates.md) → [design.md](design.md) → [voice-bible.md](voice-bible.md) → [teardown-pointandclick.md](teardown-pointandclick.md). Plus the scripted world: [vignettes/bug-031-penultima/script.md](../vignettes/bug-031-penultima/script.md).

## What to build
A single self-contained `demo/poc.html` (no build step), low-fidelity, **inferred non-animated protagonist**, placeholder visuals, one consistent verb grammar. Recommended slice: **the abandoned game *Legends of Aranor*, Kingdom of Penultima, ticket BUG-031** — reuse the existing (loved, proven-funny) material rather than writing a new world, so the POC tests the *loop*, not new content.

Demonstrate the full loop end-to-end:
1. **Frame.** You're the Debugger at the studio; the bug tracker shows `Legends of Aranor — BUG-031`; you enter the abandoned game.
2. **Inspect (Lens 🔍).** Clicking the Lens on characters/objects returns *funny, diegetic* state cards (not raw JSON): Vexmourne `weak to: being taken seriously`; the binder as a locked `script` object; the meteor `targets: hero_mark, miss_margin: 1 handspan`; the worn footprints as `safe_zone`. Inspect is the comedy-delivery *and* the puzzle-reveal *and* the hint system.
3. **A fair puzzle (not a VN choice).** Solve it by reasoning over what the Lens reveals — e.g. the quiet third path: Lens reveals the meteor `targets: hero_mark`; the **Spanner 🔧** patches `targets → (none)`, defusing the Final Battle non-violently. Include a soft hint + a "stop digging" signal (fairness doctrine). Keep the emergent **bonk** as the tier-8 "am-I-allowed?" option.
4. **The bill (the cost).** Closing `BUG-031` opens `BUG-047: Dreadlord has discovered sincerity` — show the cost, the running joke that is the thesis.
5. **Antagonist cameo (optional but valuable).** **George** (the Fixer; renamed from AUTOPATCH, after George Boole) appears and *helpfully* offers to fix it for you / closes something you wanted left open. Plants the villain in 20 seconds.

## Constraints / bars (non-negotiable)
- **Floor effect:** nothing mood-killing. Placeholder-and-honest beats ugly-and-committed; commit **no character art**.
- One input grammar; every interaction self-teaches in <30s.
- **Voice distinctness** (Strip-Names test), **fairness** (no moon-logic; hint + stop-digging), **specificity** (the gel-pen layer).
- Everything is **candidate**; don't over-build; find the nuggets, cut the rest.
- Verify it runs (preview tools), then commit + push.

## Explicitly NOT in this POC
The overworld/studio map, multiple worlds, the Reviewer (RUBI), the full WONTFIX-cascade finale, the metroidvania spine. Those come later. This is one world proving one loop.

## Open choices the builder can make
- Reuse Penultima (recommended) vs. a fresh tiny game.
- Which single puzzle is the spine of the slice (the patch-the-meteor path is recommended as the clearest inspect→patch demonstration).
- Whether to include the George (Fixer) cameo now or stub it.
