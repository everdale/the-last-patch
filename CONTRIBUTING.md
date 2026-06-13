# Contributing — the toolbox (not a pipeline)

The earlier version of this file was a nine-gate assembly line every world "must pass in order." That was a mistake, and it's exactly the trap Håkan named: **if five worlds all run the same checklist, the player feels the checklist.** "Find thing → use thing → solve puzzle → talk → minigame" repeated is death by structure.

So this is a **toolbox**. A world reaches for whatever tools build *that* world best, and deliberately differs in shape from its neighbours. There is no required sequence and no required set. The only things that don't vary are a handful of non-negotiables below.

> Before adding anything, read [docs/status.md](docs/status.md). Most of the design is **candidate**, not canon. New ideas enter as candidates; don't write them as settled.

---

## The non-negotiables (these don't vary; everything else does)

1. **It's a game, not a slideshow.** Real interaction and reasoning, not a dialogue tree with a delay.
2. **Comedy is character + situation.** Bits, not quirks; enacted, not read; cut anything that needs a second read. (See [docs/humor-doctrine.md](docs/humor-doctrine.md).)
3. **Voices stay distinct; worlds feel distinct.** Run the Strip-Names test ([docs/voice-bible.md](docs/voice-bible.md)). No house-wit collapse.
4. **Be fair.** No moon-logic. Every non-obvious solution has a discoverable hint and a "you're done here" signal.
5. **Vary the shape.** A new world must differ *structurally* from the ones before it, not just cosmetically.
6. **Draft long, cut half.** First-draft comedy regresses to wacky. Volume is raw material; the product is what survives the red pen.

That's it. Six. Everything below is optional technique.

## The toolbox (reach for what fits; no world uses all of it)

- **Puzzle techniques** — a *palette*, not a quota: low-hanging fruit, standalone reasoning, dialogue-hidden hints, inventory combination, inspect-gated, patch-a-value, power puzzles, emergent "am-I-allowed" gags. ([docs/puzzle-design.md](docs/puzzle-design.md) describes them — as options to draw from, **not** a list to complete.)
- **The debugger kit** (candidate) — Lens to read hidden state, Spanner to write it. ([docs/the-mechanic.md](docs/the-mechanic.md).)
- **Voice Cards** — fill before writing a character so they diverge by construction.
- **The world's verb + a return shortcut** — *if* this world earns a power and *if* the spine wants one. Not mandatory. ([docs/world-traversal.md](docs/world-traversal.md).)
- **The bill** — *if* we keep the "every fix has a cost" thesis, write the second ticket your fix opens.

### Vary the shape — concretely
Worlds should not be the same machine in different paint. Some legitimate, *different* shapes:
- a **dense puzzle box** (many small interlocking puzzles, little talk);
- a **single big setpiece** (one elaborate problem, earned over the whole world);
- a **dialogue-led** world (the "puzzle" is social — who to believe, what to repeat, à la a deduction game);
- a **toy** world (you're mostly playing its genre's own game, lightly subverted);
- a **trick** world (it breaks its own rules — the emergent tier carries it).
Pick a shape that suits the world's one joke. Then make the *next* world a different shape.

## Scope & gating — managing the move-space

Håkan, point 2: Monkey Island gates by episode, so at any moment your plausible moves are few and legible — you're never staring at "anchor on Mêlée or Blood Island?" An open world that's *always* fully open turns getting-stuck into brute-forcing a huge permutation space, which is misery.

Principles:
- **Bound the active combination set.** At any point, the set of things that could plausibly combine should be small enough that reasoning beats brute force. Scope is a resource you spend deliberately, not an accident.
- **Gate in controlled chunks.** Finishing a beat/world opens the next and quietly closes the last, the way a chapter does. The player's mental "what can I try right now?" stays short.
- **Signpost the frontier.** The player should always be able to tell *which* problem is the current one. Stuck should mean "I don't see the solution," never "I don't know which of forty rooms the solution is even in."

## Inventory & affordances — the Day-of-the-Tentacle problem

Håkan, point 3: shared inventory across a cast/across worlds is brilliant *and* frustrating — "do I have to test this random item against all three characters / all five worlds?" Mitigations (trade-offs, not defaults):

- **Per-world scoping, used sparingly.** A world may reject out-of-place items (the RPG world shrugs at modern/future gadgets). This shrinks the search — but it also taxes absurdist comedy (no sonic blowtorch on the medieval trapdoor). Spend it only where the frustration outweighs the gag.
- **No false affordances.** Håkan hates scenery that *looks* interactive but is a distraction. Default: if a thing can be selected, it should matter (or be clearly, sparingly, flavour). Aim to balance worlds so we don't *need* filler interactables at all.
- **Non-interactable → shortcut.** The preferred way to express a newly-opened path: a thing you genuinely *couldn't* select before (a door, a grate) becomes usable once unlocked from the other side. Clean, legible, no red herrings.
- **The Lens is the anti-distraction tool, not a source of distraction.** Inspecting plain scenery returns a clearly *terminal* card ("just a wall") so the Lens tells you what's inert. Used this way, inspect *reduces* false affordances instead of making everything look live. (This is the answer to "doesn't inspect-everything make everything seem interactable?" — no, if inert things read as inert.)

## A note on examples vs. specs

Håkan, point 6: when he sketches a mechanic ("a Shakespeare-quoting NPC could hint a clock setting"), that's an *illustration of a principle*, not a build order. Extract the nugget (hints can hide in dialogue; bound the search), don't ship the literal example as canon. The Bard's Clock demo is tagged **example only** in [docs/status.md](docs/status.md) for exactly this reason.

## If you are an AI contributor

Two failure modes, both yours:
- **Sameness.** One wit, one rhythm, one joke shape across every character and world. The Voice Cards, the Strip-Names test, and "vary the shape" exist to fight *you*. When unsure, make two things **more different than feels natural** — the pull is always toward collapse.
- **Over-commitment.** You will tend to write candidates as if decided, and to over-build throwaway examples into enshrined deliverables. Don't. Mark new ideas candidate; check [docs/status.md](docs/status.md); and when in doubt, **cut** — the brief is to find the golden nuggets, not to produce volume.

## Repo layout

```
docs/            doctrine + the status register (read status.md first)
vignettes/       one folder per world; _TEMPLATE.md is a light worksheet, not a mandate
demo/            low-fi logic/dialogue prototypes (placeholder visuals, inferred protagonist)
```
