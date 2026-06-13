# Puzzle Design — a palette, not a checklist

> Status: the *tiers* below are a useful vocabulary; the earlier "distribution rule" (quotas like "≥4 of 8 tiers, no 3 in a row") has been **retired** as too rigid — it was a formula, and formulas are the thing we're avoiding (Håkan, point 1). What survives is the *spirit*: vary the diet, don't go one-directional. Reach for tools that fit the world, not a quota to fill.

Håkan's fear, stated exactly: the monkey-wrench logic in Monkey Island is hilarious *because the rest of the game isn't that.* "If basically the whole game was just that kind of logic the game would become quite bad." A great adventure is a **balanced diet** of puzzle types — some obvious, some clever, some hidden in talk. This doc is the *menu you order from*, world by world, choosing what suits that world's one joke.

## The eight tiers

Every puzzle in the game is tagged with one of these. (Tags are tracked per vignette so we can audit the mix — see the distribution rule below.)

| # | Tier | Player feeling | Canonical example |
|---|---|---|---|
| 1 | **Low-hanging fruit** | "Obviously." *(satisfying click)* | Knife on the rope holding the curtain. Teaches verbs, builds confidence, sets rhythm. |
| 2 | **Standalone reasoning** | "Let me think… got it." | You find a thing, interact immediately, solve it with logic — no item, no hint. A balance scale; a sliding block; ordering four portraits by the dates on them. |
| 3 | **Dialogue-hidden** | "Wait — he *told* me." | The Bard's Clock. A number is buried in flavour talk; the solution is to *listen*. (See fairness below.) |
| 4 | **Inventory combination** | "What if I…" | Classic use-X-on-Y, but mined from a real inventory against a real world, not a 3-button menu. |
| 5 | **Inspect-gated** *(Lens)* | "I'd never have seen that." | The affordance is invisible until you Lens it: a hairline seam, an NPC's hidden `weak to:`, a settable value. |
| 6 | **Patch** *(Spanner)* | "I can just… change it?" | Inspect reveals an editable value; you torque it. `gate.opens_at`, the bolted hand, a wall's `solid: true`. |
| 7 | **Power puzzle** | "*This* is what Pause is for." | Uses an earned verb: freeze a falling moment, Noclip a fake wall, Save-Scum to learn a combination, Skip a guard's patrol. |
| 8 | **Systemic / emergent** | "…am I *allowed* to do that?" | The game never suggests it. The bonk. Watering a plastic fern. Pressing the forbidden idle button. The funniest tier; the rarest; the one the player authors. |

Tiers 5–8 are the ones unique to *this* game. Tiers 1–4 are the classic adventure backbone — we keep them because they're the floor, the low-hanging fruit, the breathing room that makes the clever ones land.

## Instincts, not rules (the retired quota)

The earlier draft hardened these into a "distribution rule" with numeric quotas. That was the formula trap again — so treat them as **instincts a good designer already has**, applied with judgement per world, not gates a reviewer counts:

- **Don't go one-directional.** A world that's all patch puzzles is as dull as one that's all emergent cleverness. Mix.
- **Pace by contrast.** After a head-scratcher, a quick win breathes. Sameness in a row is the thing to feel for.
- **Welcome gently; never wall the story.** Early puzzles should be inviting; the *story-clear* path should never be the hardest thing in the world (save brutal for optional mastery).
- **Emergent gags are seasoning.** The "am-I-allowed?" trick (the bonk) is special *because it's rare*. Lean on it once and it lands; lean on it repeatedly and players pixel-hunt for tricks instead of inhabiting the place.
- **Teach a verb easy before gating behind it.**

None of these is a quota, and a world is free to break one on purpose if the world's one joke demands it. The only hard test is the one at the bottom of this doc.

## Fairness doctrine (so "clever" never means "unfair")

Adventure games die on moon-logic. Three guarantees, every non-obvious puzzle:

- **The soft hint exists in the world.** A character, a Lens card, or an object states the logic if you seek it. (Bard's Clock: the Bard *says the number*; the playbill gives the reference; the Lens explains the mechanism.)
- **The "stop digging" signal.** Håkan's exact request: when one item in a set is the answer, something tells you the set is finite and you've found it. The Critic: *"one line in a hundred holds water — you'll know the one when it's useful, and you may stop your digging there."* This kills the failure mode where the player keeps trying the other four Shakespeare quotes forever. Generalise it: every "find the one X" puzzle ships an NPC or card that bounds the search and confirms the hit.
- **Escalating hint button.** A diegetic last resort that ramps: nudge → mechanism → near-spoiler → full chain. Using it costs nothing but a mastery tag (completion-without-hints is its own tier-2 mastery). Implemented in the proto.

## Worked example: retrofitting Penultima into real puzzles

[BUG-031](../vignettes/bug-031-penultima/script.md) currently plays as VN-with-a-bonk. Same story, re-shaped through the tiers:

- **Tier 1 (low-hanging):** the east door is stuck; *push* it (it yields on the third try). Trivial, sets the verb.
- **Tier 5 (inspect):** Lens the meteor → `miss_margin: 1 handspan`, `targets: hero_mark`. Lens the floor → the two worn footprints glow as `safe_zone`. *Now* the "stand in the feet / do nothing" beat is something you discovered, not were told.
- **Tier 3 (dialogue-hidden):** the correct cue line ("the morning does not negotiate") is gettable by listening to Vexmourne's notes and the grandfather's binder, not by trying all three buttons.
- **Tier 6 (patch):** Lens the binder → it's a `script` object with a locked `role: villain`. The *quiet* solution (besides the bonk) is to patch the meteor's `targets` from `hero_mark` to nothing — defusing the fight non-violently, a third path with its own ending beat.
- **Tier 8 (emergent):** the bonk. One per world. Stays exactly as written.

Result: the same fifteen minutes, but now the player *acts* through five different kinds of thinking instead of advancing text. The jokes are unchanged; they're now things you *do*.

## The one-line test for any new puzzle

> Could a player who muted all dialogue still, in principle, solve this by looking and reasoning? And could a player who skipped all puzzles still laugh?
If **neither** is true, it's a cutscene wearing a puzzle costume — cut it or rebuild it.
