# World Traversal — discovery is long, return is instant

Point 7, named exactly: Sea of Stars (and most good RPGs) make *first* discovery a journey, but once you've cleared a place, getting back is fast — you don't walk fifteen screens to re-reach a toy you love. If the racing-world has a racer a player wants to revisit, the first trip earns the right to a shortcut; every trip after is a hop. This doc makes that a law at two scales, and ties the shortcuts to the game's own verbs so traversal upgrades feel earned rather than administrative.

## The principle

> **The map contracts as you master it.** Distance is a thing you spend once, to buy the right to never spend it again.

This also serves the completion KPI ([design.md §1](design.md)): busywork backtracking is exactly the "abandoned at 60%" failure mode. And it serves the light-metroidvania spine — the world reopening behind you is real, but never a chore.

## Scale 1 — between worlds (the overworld)

- **First arrival is a journey.** Reaching a new genre-land for the first time winds through connective screens. That traversal is content: roadside gags, a slime queueing for tomorrow, the texture that makes the place a *place*.
- **Clearing a world's core ticket drops a Warp Node.** A fast-travel anchor (thematically skinned per genre: a save-crystal, a warp pipe, a fast-travel campfire, a `// TODO: real fast travel` placeholder that works anyway). From then on, the world is one hop from the map.
- **The shortcut is itself a power, not a menu.** Where possible, the *means* of fast return is an earned debugger verb, so traversal and progression share one vocabulary:
  - **Cutscene Skip** collapses the long dialogue-corridors you've already seen.
  - **Noclip** opens the wall that made the first route long.
  - **Save Scum** bookmarks a spot and snaps you back to it.
  - **Patch** (endgame) can rewrite a region's `distance` rule outright.
- **Result:** the second visit to Penultima isn't "walk the road, watch the slime, cross the square, enter the castle." It's: warp to Penultima → you're at the throne room. The road still exists for anyone who wants it; it's just no longer mandatory.

## Scale 2 — inside a world (re-entering a cleared vignette)

- **Beaten levels fast-forward their own setup.** Re-enter a solved vignette and the intro cutscene, the tutorial verb-teach, and the diagnosis chatter are skippable/auto-skipped (the Penultima swirl, the binder explanation). You drop straight into the part you came back for.
- **Solved puzzles stay solved.** The curtain stays cut; the gate stays open. Returning for a *mastery tier* doesn't re-watch the curtain fall — it starts at the new challenge.
- **Mastery content lives behind the now-short path.** Grenadine's higher rubric scores, the racer's "actually lose" challenge, speedrun/no-hint clears — all reachable in seconds on return, never gated behind re-traversal.

## The verb-shaped shortcut table

| You earned… | …so revisiting becomes |
|---|---|
| Cutscene Skip (Penultima) | hold ⏩ through any corridor you've seen; patrols and timers fast-forward |
| Noclip (Early Access Swamp) | the long way around a `[coming soon]` wall is now a straight line through it |
| Save Scum (Roguelike land) | set a bookmark anywhere; return collapses to a keystroke |
| Pause (fighting-game land) | freeze a hazard-corridor and stroll the cleared route |
| Patch (endgame) | rewrite the rule that made the place far |

## Design rules (review-enforced)

1. **No mandatory re-traversal.** If a player must cross more than ~2 screens to reach previously-unlocked content, the world is missing its Warp Node. Reject.
2. **The shortcut is diegetic and ideally a verb.** A bare "fast travel" menu is the fallback, not the goal; prefer a shortcut the player *unlocked the means for*.
3. **The long road survives.** Never delete the scenic route — some players (and mastery 100%-ers) want it. Make it optional, not gone.
4. **First-trip length is a content budget, not filler.** If the connective screens aren't carrying jokes or texture, shorten the first trip too. Distance must always be paying for something.

## How this reshapes the map over a playthrough

Early game: a sprawling overworld you traverse screen by screen, learning its geography and its gags. Mid game: a constellation of Warp Nodes — the sprawl is still *there* but you skip across it. Late game: with Patch, you start editing the connective tissue itself. The journey was the point on the way out; the contraction is the reward on the way back. The player feels themselves getting *powerful over space*, which is exactly the debugger fantasy applied to the map.
