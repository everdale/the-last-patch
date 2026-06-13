# The Last Patch

> A comedy point-and-click adventure where you play the **Debugger** — the one person who can step *inside* broken games and fix them from within. Every land is a game with one broken rule. **Every fix opens two tickets.** The last patch might be the decision to stop patching.

**A candidate USP (auditioning):** *the inventory is a debugger — look at anything to see how it really works, then break it on purpose.*

> ⚠️ **Most of this repo is exploration, not settled design.** Read [docs/status.md](docs/status.md) first — it marks what's *decided* vs. *candidate* vs. *throwaway example*. The earned verbs, the specific worlds (Penultima etc.), and most of the structure are candidates we're auditioning, not commitments.

---

## ▶ Play the prototypes (just open the files)

These are **low-fidelity logic/dialogue prototypes** — placeholder visuals, an *inferred* (non-animated) protagonist, no committed art. They exist to test interaction, dialogue, and structure, not to show how the game will look.

- **[demo/index.html](demo/index.html)** — **BUG-031, the Kingdom of Penultima.** A narrative vignette: a JRPG throne room where the Final Battle has been in rehearsal for four hundred years. Two solution paths (perform the show, or just… hit him with the wrench), with consequences that write you letters. *A tone test.*
- **[demo/puzzle-proto.html](demo/puzzle-proto.html)** — **the Bard's Clock.** A **disposable spike**: built only to prove a world can be a real point-and-click puzzle and not a visual novel. The clock itself was a throwaway example — keep the *principles* (hints can hide in dialogue; bound the search), not the puzzle. Tagged *example only* in [status.md](docs/status.md).

Both run as plain HTML — no build step. Open in any browser.

## 📖 Read the design

Start with the design doc, then the mechanic, then the doctrine docs.

- **[docs/design.md](docs/design.md)** — what the game is and what it's *for* (completion & memory, not retention).
- **[docs/the-mechanic.md](docs/the-mechanic.md)** — the inventory-as-debugger USP; why it's a game, not a visual novel; the Lens & the (comically oversized) Spanner.
- **[docs/humor-doctrine.md](docs/humor-doctrine.md)** — bits not premises; jokes enacted not read; the kill-rate.
- **[docs/puzzle-design.md](docs/puzzle-design.md)** — the 8 puzzle tiers and the distribution rule that keeps variety from collapsing into one trick.
- **[docs/voice-bible.md](docs/voice-bible.md)** — Voice Cards + the Strip-Names test, so no two characters sound alike.
- **[docs/world-traversal.md](docs/world-traversal.md)** — discovery is long, return is instant; the map contracts as you master it. *(candidate)*
- **[docs/tickets.md](docs/tickets.md)** — a candidate menu of worlds (examples + tone tests, **not** a committed roster).
- **[docs/status.md](docs/status.md)** — ⭐ **the commitment register**: decided vs. candidate vs. example vs. open question. Read this to know what's real.
- **[docs/teardown-pointandclick.md](docs/teardown-pointandclick.md)** — differential teardown of the genre: what sinks entries (MI4's controls + Monkey Kombat, moon logic, **the Floor Effect** — GK3/MM9 breaking their load-bearing pillar, the meta-ending that *severs*) vs. carries them, and the deliberate blend that makes us novel.
- **[docs/the-antagonist.md](docs/the-antagonist.md)** — *(candidate)* the villains: **two AIs** the studio bought — a cheerful **Fixer** that can't stop improving and can't WONTFIX, and a Grok-waifu **Reviewer** that pans everything. The two hollow halves of taste. Includes the seahorse-emoji exploit and a written first-contact scene.
- **[docs/ending-candidates.md](docs/ending-candidates.md)** — *(candidate)* the end-game: the **WONTFIX cascade** — "fix spawns two" as a *toy* you play until you choose to stop — turned into the weapon that beats the AI (a thing that must fix everything drowns where every fix opens two). Includes a worked, funny cascade.

## 🛠 Build a world

- **[CONTRIBUTING.md](CONTRIBUTING.md)** — the **toolbox** (not a pipeline): six non-negotiables, then optional technique. Built so worlds vary in *shape*, not run a checklist.
- **[vignettes/_TEMPLATE.md](vignettes/_TEMPLATE.md)** — a light worksheet to start a world (skip what doesn't fit).
- **[vignettes/bug-031-penultima/script.md](vignettes/bug-031-penultima/script.md)** — the first scripted world, as a tone test (both paths, the letters, an appendix).

## Status

Early exploration. A candidate USP, a couple of tone tests, and a doctrine that's deliberately held loose. **Nothing is locked** — see [docs/status.md](docs/status.md). Next step is a **POC** ([docs/poc-brief.md](docs/poc-brief.md)). Open decisions still in play: how heavy the spine is, and which flavour of the AI finale rings truest.

## The pitch, slightly longer

You're a Debugger at a game studio with a graveyard of **abandoned, unfinished games** — and you fix them from inside. Each is a specific title with its own soul: *Legends of Aranor*, whose villain has rehearsed the final battle for four centuries because the hero transferred to another game two days before opening night; a horror game that isn't scary because the monster ordered a mirror-maze to feel surrounded and became a narcissist; a racer with one driver who physically cannot lose and is hollow inside. You arrive with a magnifying glass and a wrench, and slowly you learn that every fix ruins something too. Meanwhile the studio buys **two AIs** to finish and review the backlog without you — one that improves everything until it's beige, one that pans everything to ash — and they're coming for your job. You beat them with the one thing they'll never have: knowing when to leave a bug alone.

Nobody's made the warm one. This is the warm one.
