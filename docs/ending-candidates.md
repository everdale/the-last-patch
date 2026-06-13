# The End-Game — the WONTFIX cascade

> 🟡 **Candidate / exploratory**, and a **revision** of an earlier, heavier draft. Håkan pushed back: does this need to be a *meta*-ending at all? It doesn't. This version keeps the good salvage (the "fix spawns two" idea, a WONTFIX verb, causal legibility, a fairness signal) and drops the fourth-wall sermon. The old meta-heavy material is demoted to a footnote at the bottom.

## The pivot, in one line

From a **fourth-wall meta-ending** (risky: the genre's most-stepped-on rake) to a **diegetic genre-nod**: a climax that's funny, mechanical, and *in the fiction* — a loving send-up of bug-tracker/QA culture and of the point-and-click genre's own sins.

What we keep, and how its role changes:
| Idea | Old role (cut) | New role (kept) |
|---|---|---|
| "Every fix opens two tickets" | a thesis the game *states* | a **toy** the player *plays with* because the spawned bugs are fun to read |
| WONTFIX | a solemn metaphor | a literal **verb**, and the climactic decision |
| Causal legibility | — | end-game bugs **clearly caused by your specific earlier fixes** (Wally callbacks) |
| Anti-moon-logic signal | — | a bug whose requirements are explicitly **unattainable**, with an NPC saying *don't bother* |

Dropped or demoted: the "you and The Update are the same verb" sermon; the "you are the bug" reveal; "hand back the verb"; the meteor "no input" rhyme (at most a faint grace note now, cuttable).

## The shape

The final world is **The Backlog** — the adventure/QA genre itself, treated with the same affection as every other genre-land. Your past fixes have come due, gathered as a ticket queue. Each ticket offers **[FIX]** and **[WONTFIX]**.

- **FIX** closes it and *spawns two new, dumber bugs* — hand-authored, escalating, full of callbacks. Reading the cascade is the reward. You can keep going as long as it amuses you; pace belongs to the player.
- **WONTFIX** closes it clean — no spawn.
- The queue teaches itself: the first bug looks easy and *important* (new players are blocked!), tempting a FIX. You fix it, the chaos blooms, you get the joke — and now you understand the other button.
- It ends on one last ticket: **BUG-001 — "world contains bugs."** `[FIX]` would begin the whole cascade at world-scale. `[WONTFIX]` is the ending: you let the world keep its bugs — its scars, its changes, its *soul* — close the tracker, and go home. The thesis lands as a *button press and a joke*, never a speech.

## The comedy proof (a real cascade — judge the writing, that's the whole bet)

> **BUG-209** — Dreadlord weeps through new-player onboarding. Tutorial unreachable. *(you gave Vexmourne sincerity)* &nbsp; `[FIX]` `[WONTFIX]`

*You pick **FIX**. "Patch deployed: assigned the Dreadlord a therapist." Two tickets open:*

> **BUG-231** — Therapist is now the most beloved party member. Players refuse to fight the final boss so they can keep doing his sidequests.
> **BUG-232** — Dreadlord and therapist have launched a podcast. Episode 1 runs four hundred years. Early listeners say it "slaps."

*You can't help it. You **FIX** BUG-231. "Patch deployed: therapist written out of the party." Two more:*

> **BUG-240** — Review-bombing in progress: "YOU KILLED GARY." #JusticeForGary is trending in three kingdoms.
> **BUG-241** — Dreadlord has relapsed. Now insincere *and* crying. Critics are calling it his best work.

*And, a few fixes deeper, sitting in the queue:*

> **BUG-250** — RESOLUTION BLOCKED. Requires: the **Golden Wrench** (deprecated), **Senior Approval** (Senior has left the company), and **Three (3) Business Days** (it is a holiday weekend).

*Dennis — somehow here, holding a clipboard, an honour — leans over:*

> **DENNIS:** Don't even start on that one. The Golden Wrench got deprecated two patches back, Senior's gone, and nobody's approving anything till Monday. Some tickets you just… let live. Mark it WONTFIX. Go home.

*And there it is — the button you've had the whole time. You start marking them WONTFIX. Each one closes clean. The chaos drains, not by fixing, but by declining. Until only BUG-001 is left.*

## The fairness signal (Håkan's point, and the anti-GK3)

BUG-250 is the load-bearing fairness beat: a bug that *looks* like it wants a three-item fetch-quest, and the game **immediately tells you the items are unattainable and to stop.** This is the exact inverse of moon logic — instead of letting you grind for hours on a cat-hair mustache, an NPC says "those are never coming; WONTFIX it." It's also a perfect QA-culture joke (deprecated tooling, the senior who left, the holiday weekend). Every "go get X, Y, Z" temptation in the end-game ships with its own "don't bother" so nobody mistakes the toy for a chore.

## Two framings — your call

**(i) You had WONTFIX all along.** It's been a low-stakes option the whole game (you've WONTFIX'd cosmetic junk: *"BUG: grass clips slightly. WONTFIX: nobody cares"*). The end-game realization is that you can apply it to something that *matters* — the power to stop was always in your hand; you just kept choosing to fix. *More resonant, foreshadowable, recontextualises your whole journey without a twist.* **Recommended.**

**(ii) You gain WONTFIX in the chaos.** You never had it; in the fix-one-spawn-two meltdown, you unlock it, and the ending that looked impossible becomes a formality. *Cleaner as a classic adventure beat (impossible wall → earn the verb → wall dissolves), slightly less thematically loaded.*

Both work. (i) makes the ending a *choice you finally dare to make*; (ii) makes it a *power you finally earn*. Pick the feeling.

## Why this beats the earlier draft (audited against our own docs)

- **Recontextualise, not sever** ([teardown D](teardown-pointandclick.md)): fully diegetic; nothing the player did is invalidated. ✓
- **Not preachy:** the thesis is delivered as a mechanic and a punchline, never a monologue. ✓
- **Floor effect** ([teardown E](teardown-pointandclick.md)): the humor pillar carries it — which means the **bug-writing is the load-bearing craft**, and that's our strength. ✓ (and our exposure — see risk.)
- **Genre nod, warm:** the finale lets the adventure genre look at itself with affection, consistent with how every world treats its genre.

## What this lets us cut or demote (the brief was: find the nuggets, cut the rest)

- **The Update** villain becomes *optional* — the antagonist is now your own compulsion to fix. (Cleaner; The Update was candidate anyway.)
- **Patched Anonymous** becomes optional / a lighter mid-game beat rather than the thesis hammer.
- **The meteor "no input" rhyme** — at most a faint echo (WONTFIX *is* a kind of declining-to-act), cuttable.

## Risks & the cheap gate

- **The Monkey-Kombat risk:** any repeated mechanic can grind. Antidotes: the cascade is **hand-authored** (not procedural junk), **escalating**, **callback-rich**, and **"go home" is always one WONTFIX away**. If reading bugs ever feels like work, it's failed.
- **Anti-climax tone:** "mark it WONTFIX and go home" is deliberately wry and small, not an epic boss. That fits our warm/completion-focused tone — but pair the final BUG-001 with one quiet emotional beat (you're choosing to let the worlds keep their scars) so it resonates, not just shrugs.
- **The gate (paper-cheap):** write **3–4 complete cascade chains** and read them cold. If they're funny on the page, the mechanic is real. If they're not, no engine work would have saved it. This is a writing bet, decided on paper first.

## Open questions for you

1. Framing **(i)** or **(ii)**?
2. Is the final world literally *"the bug tracker / The Backlog,"* or a last genre-land whose one bug happens to be the cascade?
3. Keep a small emotional beat on BUG-001, or play it pure-dry?

---

### Footnote — the heavier alternatives we stepped back from
Earlier drafts proposed a fourth-wall ending: *you and The Update are the same verb at scale*; *you are the bug the world filed a ticket to fix*; *spend your last patch giving worlds the ability to refuse you*. Recorded here only so the reasoning isn't lost. They're higher-concept and higher-risk (sever-prone, preachy), and the WONTFIX cascade delivers the same "the last patch is the decision to stop" payload more cheaply, more funnily, and without touching the fourth wall. Park them; don't build them.
