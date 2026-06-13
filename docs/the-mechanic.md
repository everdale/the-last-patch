# The Mechanic — what makes this a *game*, and the USP

> 🟡 **Candidate, not decided** ([status.md](status.md)). The inventory-as-debugger idea below is my strongest current *proposal* for the USP — promising and unproven. It could change form entirely, or lose to something better. What's genuinely settled is only the problem it solves (it must be a game, not a visual novel), not this particular solution.
>
> Disposable proof-of-concept: [demo/puzzle-proto.html](../demo/puzzle-proto.html) — a spike showing the idea *can* be a game. The clock puzzle is throwaway; the mechanic is the point.

## The problem this solves

The first vignette ([BUG-031](../vignettes/bug-031-penultima/script.md)) reads like a visual novel. Diagnosis (Håkan's, and correct): when "use X on Y" is one of three buttons in a dialogue tree, it's trivial — you'll click all three in ten seconds. The puzzle isn't a puzzle; it's a menu with a delay. A real adventure game has an **inventory you can point at the whole world**, so the interesting question is *which* of many things to try on *which* of many things — a search, not a shortlist.

So the core loop can't be "advance text / pick from 3." It has to be a point-and-click with a real verb space. And the verb space, to be *unique* (point 6) rather than another Monkey Island reskin, comes from the one fantasy nobody has mechanised warmly:

## The USP, in one line

**The Last Patch is a comedy point-and-click adventure whose inventory is a debugger. Look at anything to see how it really works — then break it on purpose.**

Not "you travel between games" (Wreck-It-Ralph, Evoland — the setup, which is only *somewhat* novel). The novel part is the *verb*: you carry the tools of a debugger into worlds that don't know they're games, and you can **read and write their hidden state.** That's a mechanic no warm comedy adventure has shipped. (Pony Island / The Hex touch "hacking the game" but as horror; *There Is No Game* plays with the UI, not the world's state. The cozy one is unbuilt.)

## The kit (and point 4: wrench → spanner, plus the Lens)

Two foundational tools. Håkan is right that a *spanner* (open-end wrench, UK term) reads as plumbing, not debugging — and that the debugger's natural icon is a magnifying glass. So we give him **both**, with distinct jobs:

### 🔍 The Lens — *INSPECT* (innate; it's how a Debugger sees)
Point it at anything and the world stops being a flat picture: it reveals the object's hidden state as a little card. **Crucially, the card is never raw JSON** — that fails the fourteen-year-old test (see [humor-doctrine.md](humor-doctrine.md) §6). It's rendered diegetically, and the rendering is itself a joke:

```
VEXMOURNE IX
  role: Villain (rehearsing)
  last genuine emotion: none on record
  weak to: being taken seriously
```
```
THE CRITIC
  performances rated: 14,000
  joy: 0.0
  currently: deducting points for this card
```

The Lens does three jobs at once — which is the Sea of Stars "every aspect pulls weight" standard:
1. **Puzzle engine.** Affordances are *hidden in state*, not listed in a menu. You must look to find them. That converts "pick from 3" into "inspect the room, form a theory, test it." A search space.
2. **Comedy delivery.** Every inspect result is a punch-up surface — the specificity layer (doctrine §8) lives here, and it's optional, so it never forces a second read (doctrine §7).
3. **Fairness.** It's also the built-in hint system: stuck players can Lens the relevant object and the card nudges them. Anti-frustration is baked into the core verb.

### 🔧 The Spanner — *MANIPULATE / PATCH*
The crude end of the same idea: physically adjust exposed mechanisms, and later, edit values the Lens has revealed. The **bonk is the spanner's stupidest possible use** (and a great one). Its elegant uses: loosen the bolted clock-hand so it becomes settable (proto), pry a `[coming soon]` wall, torque a value you found.

**Why does a debugger carry a giant wrench? (point 4, the comically-oversized gag.)** It's standard QA-depot issue, requisitioned through a form whose `size` field has no input validation — so it came out at `size: MAX`. Inspect the requisition slip and you can read exactly that. One gag that is simultaneously: a laugh, worldbuilding, a tutorial for the inspect mechanic (the unvalidated field *is* a bug you can see), and foreshadowing that this whole world is software with its guards down. The Lens he's always had; the Spanner is the first tool you pick up, and it lands "with a sound like a bell being told bad news."

## The earned powers are just more debugger verbs

The meta-powers from each world ([design.md §4](design.md)) aren't a separate system — they're new ways to read/write state, which is why they feel coherent and why they reopen old worlds (point 7, the spine):

| Verb | Debugger reality | Puzzle type it unlocks |
|---|---|---|
| Lens | read state | inspect-gated |
| Spanner | write state | patch |
| Save Scum | checkpoint/restore | branch-observe-rewind |
| Pause | breakpoint | act inside a frozen moment |
| Noclip | ignore collision | the wall was never real |
| Cutscene Skip | fast-forward a process | timers, patrols, speeches |
| **Patch** (endgame) | rewrite a rule | the finale verb |

## Why this fixes points 3, 5, and 6 at once

- **It's a game (3):** there's a board (the room), inventory, hidden state, and solutions you reach by reasoning. The proto is solvable only by chaining knife→curtain, hatch→spanner, spanner→clock, and a *number you have to derive*.
- **"Use X on Y" is non-trivial (5):** the Lens hides the affordances; the inventory points at everything; the space is combinatorial. The proto has red-herring quotes, wrong hours, and tools that don't work where you'd guess.
- **It's unique (6):** the inventory-as-debugger verb is the thing no warm adventure has done. The setup attracts; *this* keeps.

## What the Lens must never become

Programmer cosplay. No monads, no stack traces, no literal code unless the *code itself is the joke a gamer gets* (an unvalidated form field, a `WONTFIX`, a 400-day-old ticket). The register is **gamer, not engineer** (doctrine §6). If a card needs a CS degree to be funny, cut it.
