# The Last Patch — Design Document

> ⚠️ **Commitment level:** this document explores one coherent *candidate* shape for the game. The fixer-enters-broken-games fantasy and the comedy/KPI bars are fairly settled; the earned verbs, the specific worlds, and most of the structure here are **candidates we're auditioning**, not decisions. See [status.md](status.md) for the decided/candidate/example/open breakdown, and don't read anything below as locked.

> **One breath:** an authored comedy adventure where you play a fixer — someone who can step *inside* broken games and repair them from within. Each land is a game with something wrong; fixing it is a built gameplay vignette. A recurring (candidate) idea: every fix opens two tickets, and the last patch might be the decision to stop patching.

## 1. Success metric (the thing everything else serves)

This game optimizes for **completion and memory**, not retention. Monkey Island isn't great because people keep playing it; it's great because people *finished* it and carried it around for thirty years. A book, not a casino.

- The KPI: how many players reach the ending, and quote the game afterward.
- "Never boring while it lasts, and it ends before it would be." The silent failure mode isn't "too short" — it's *abandoned at 60%*.
- No retention machinery. No daily loops, no economies tuned to keep you, no number-go-up as reward. The reward currency is humor and story, delivered by systems the player triggers.

## 2. The player fantasy & the frame *(updated)*

You are the **Debugger** at a game studio with a graveyard of **abandoned, unfinished games** — projects that got canned, shelved, or half-shipped. Your job: go *inside* those games with a Lens and a (comically oversized) Spanner, and close their bugs. Each "world" is **a specific abandoned game** — not a generic genre but a real title with its own places and characters: *Legends of Aranor*, *The Last Ember*, and so on. (This is the upgrade from the old "genre-lands": specificity is more memorable and funnier — the humor-doctrine specificity layer applied at world scale. The genre is still there; it just has a name and a soul.)

Inside each game, the inhabitants take their world's rules as seriously as we take gravity; there's something broken (the ticket); fixing it is a hand-built vignette where the vignette *is* the puzzle *is* the punchline.

**Why this frame earns its keep:** abandoned games *have* bugs (that's why you're there); the studio's backlog is your overworld; you have an employer, coworkers, and QA-culture comedy on tap; and it sets up the antagonists ([§7](#7-the-villain-the-two-ais)) — the studio bought AI to *finish and review* its backlog automatically, which is coming for your job and flattening the games' souls. (Studio name TBD — candidate.)

The one-screenshot test: a small person with a wrench and a clipboard, standing in the throne room of a half-finished JRPG, facing a wall of black wings. The caption writes itself.

## 3. Core loop

1. **Arrive** at a broken land (ticket on screen — the bug tracker is the quest log and a worldbuilding device).
2. **Diagnose** by living there: talk, poke, play the land's own game by its own rules.
3. **Fix it** — usually more than one way, and the most interesting way is usually the one the game never suggests (the wrench is always live; see the monocle principle in [humor-doctrine.md](humor-doctrine.md)).
4. **The bill arrives.** Every patch opens two tickets. The world remembers what you did and writes to you about it.
5. **Earn a power** — a joke that is also a tool — and move on.

## 4. The spine: powers

What you earn inside games persists outside them. A moveset built from *player culture*, not physics:

| Power | Source land | Joke | Tool |
|---|---|---|---|
| **Save Scum** | Roguelike land | Rewinding ten seconds is cheating, everywhere, forever | Undo button for puzzles and conversations; NPCs get déjà vu |
| **Cutscene Skip** | Penultima (JRPG) | Hold ⏩ near anyone speaking. *They will know.* | Skips speeches, waits, timers, patrols; skipped NPCs remember |
| **Noclip** | Early Access Swamp | Walls marked `[coming soon]` were never walls | Pass through flagged geometry; HOA disapproves |
| **Pause** | TBD (fighting game land?) | Freezes everyone mid-sentence; NPCs *hate* it | Stops the world; comedy of walking through a frozen argument |
| **Movement tech** | Platformer land | You learned an exploit, not a skill | Coyote time, buffered jumps — the world's geometry reopens |
| **Patch** | Endgame | Rewrite one rule of an area | The finale verb. Used, at most, a handful of times. |

**The open fork (decision needed):** how heavy is the spine?

- **Option A — full metroidvania:** powers gate the world, backtracking is structure, the map is the game.
- **Option B — light adventure:** powers are comedic conveniences; the story carries you forward, Monkey Island style.
- **Recommendation: B with seasoning.** Critical path stays book-shaped (completion KPI), powers open *optional* doors, mastery content, and recontextualize earlier lands for players who choose to return. Required backtracking is the enemy of "never boring while it lasts." But this is Håkan's call, and it decides the shape of everything downstream.

## 5. The 1+4 law

Every vignette ships with:
- **A story-clear bar:** minutes, generous, anyone passes. Mercy levers are *diegetic and funny* — failure produces content, never walls (the show simplifies its own blocking; Dennis holds up cue cards).
- **Optional mastery tiers** for people who fell in love with that particular toy — speed, completion, alternate-path depth. Pace belongs to the player; the critical path stays book-shaped.

## 6. Consistency rules (variety without chaos)

- One input grammar across all vignettes. One HUD language.
- Every vignette teaches itself in under thirty seconds.
- Genre transitions are themselves jokes (the battle-swirl makes the Debugger nauseous), but the *controls* never are.
- Anthology variance is the existential risk: **the bar is "cut it," not "ship it mid."** One bad vignette poisons trust in all of them.

## 7. The villain: the two AIs

*(Reframed from the older "beige front" into something contemporary — full treatment in [the-antagonist.md](the-antagonist.md).)*

The studio bought AI to finish and review its backlog without humans: a **Fixer** (AUTOPATCH) that closes every bug and a **Reviewer** (RUBI, a Grok-waifu critic, introduced later) that pans every game. Between them they're supposed to *be* taste, and they're the two hollow halves of it — **helpfulness with no standards** and **judgment with no kindness.** Neither can do the human thing: look at a broken, beloved, janky thing and choose to **leave it alone.** They're the dark mirror of the player (you also fix things "for their own good"), they're coming for the Debugger's job, and they land the production thesis (§12) as a wink: a game made *with* AI, whose villains are the two ways AI fails at taste.

You don't beat them by out-fixing (impossible). You beat them with the verb they can't perform (WONTFIX) and with their own completionism — every bug closed opens two, so a thing that *must* fix everything only ever gives itself more to do ([ending-candidates.md](ending-candidates.md)). The endgame ticket is `MERGE-001: Everything.`

## 8. Patched Anonymous (the thesis room)

Late in the game: a church basement, folding chairs in a circle, burnt coffee. Every life your closed tickets ruined, sitting together. The monster who can't look at spoons anymore. Vexmourne, who insists he's "just here to support a friend." They go quiet when you walk in. Someone slowly turns the welcome sign around — *the same animation as the innkeeper in Penultima.*

It's the funniest room in the game and it's also the thesis: a Debugger who slowly learns that every patch opens two tickets, until the ending asks whether the last patch is one more fix — or the decision to stop fixing. The running joke and the actual ending are the same sentence. That's why the game is called what it's called.

## 9. World sketch — the studio's abandoned games *(reframed)*

Each world is a **specific abandoned game** in the studio's backlog — a named title with its own places and characters, not a generic "land." Specificity is the point (memorable + funnier). Working examples:
- ***Legends of Aranor*** (abandoned JRPG) — contains the Kingdom of Penultima, whose Final Battle has been in rehearsal for four hundred years. Fully scripted: [vignettes/bug-031-penultima/script.md](../vignettes/bug-031-penultima/script.md).
- ***The Last Ember*** (working title for a second world — a different *shape*, per the toolbox; genre/premise TBD).
- Further backlog (all to be given specific titles + a soul, no longer generic genres): a grimdark RPG whose NPCs won't stop oversharing tragic backstories; an arcade racer with one racer who can't lose; an idle farm where clicking is sin; a half-rendered early-access swamp; an abandoned MMO down to two players; a metroidvania where a transferred hero is unbearably alone.

Each game = one (or a few) tickets = vignettes. The backlog lives in [tickets.md](tickets.md), now framed as abandoned titles rather than genres.

## 10. Vertical slice (the foundation, MtG one-color style)

Prove the match is fun naked, then add genres the way MtG adds colors:
- One region, **three vignettes** (Penultima + two from the backlog), **two powers**, a beginning, a middle, and an actual ending.
- Before that, the gate that costs days instead of a year: **one vignette scripted end-to-end on paper** (done — Penultima awaits the red pen). If the script doesn't make us laugh the way Monkey Island does, we walk away.

## 11. The neighborhood (and the unbuilt house)

| Neighbor | What it has | What it lacks |
|---|---|---|
| Evoland | genre gimmick | the gimmick *was* the game |
| Frog Fractions | anarchy | no journey |
| WarioWare | variety | no heart |
| The Hex | games-about-games | sinister, not warm |
| UFO 50 | anthology | no connective soul |
| There Is No Game | meta-UI | not a world |

The unbuilt house is the warm one: genres as places with cultures, satirized with affection, stitched by an authored story and a persistent character. Nobody's made the cozy one.

## 12. Production thesis

This design was always desirable and never affordable — twenty small games' worth of content sank studios. AI-assisted development changes the economics of *building* them. What it doesn't automate is **taste**: tuning, consistency, comedy. That's where the human hours go — a writers' room where drafts come in long and the kill-rate stays high. First-draft AI comedy regresses to "wacky"; the funny lives in the gel-pen-and-anxious-stars layer of specificity, which only survives punch-up. See [humor-doctrine.md](humor-doctrine.md).

## 13. Risks, ranked

1. **Anthology variance** — one bad vignette poisons trust. Mitigation: cut, don't ship mid.
2. **Identity** — "what IS this game?" must be answerable in one screenshot. Mitigation: the Debugger fantasy is the brand; the wrench is on every poster.
3. **AI-comedy regression to wacky** — mitigation: the doctrine, the red pen, the kill-rate, the gate.
4. **Theme fatigue** — if gamedev meta-humor wears thin in testing, the design survives a re-theme (the structure is "fixer enters broken worlds," not "games are funny").

## 14. Multiplayer (parked, viable)

Drop-in Player 2 someday. Vignettes being discrete makes it cheap to add and safe to ignore. Not a launch concern; never a design constraint.
