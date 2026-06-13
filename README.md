# The Last Patch

> A comedy point-and-click adventure where you play the **Debugger** — the one person who can step *inside* broken games and fix them from within. Every land is a game with one broken rule. **Every fix opens two tickets.** The last patch might be the decision to stop patching.

**The USP, in one line:** *the inventory is a debugger — look at anything to see how it really works, then break it on purpose.*

---

## ▶ Play the prototypes (just open the files)

- **[demo/puzzle-proto.html](demo/puzzle-proto.html)** — **BUG-072, the Bard's Clock.** The core mechanic: a real point-and-click puzzle (inventory, the Lens 🔍 to inspect hidden state, the Spanner 🔧 to patch it). A thing you see, a thing you learn from dialogue, a tool, and a number nobody hands you. *Start here.*
- **[demo/index.html](demo/index.html)** — **BUG-031, the Kingdom of Penultima.** The narrative vignette: a JRPG throne room where the Final Battle has been in rehearsal for four hundred years. Two full solution paths (perform the show, or just… hit him with the wrench), with consequences that write you letters.

Both run as plain HTML — no build step. Open in any browser.

## 📖 Read the design

Start with the design doc, then the mechanic, then the doctrine docs.

- **[docs/design.md](docs/design.md)** — what the game is and what it's *for* (completion & memory, not retention).
- **[docs/the-mechanic.md](docs/the-mechanic.md)** — the inventory-as-debugger USP; why it's a game, not a visual novel; the Lens & the (comically oversized) Spanner.
- **[docs/humor-doctrine.md](docs/humor-doctrine.md)** — bits not premises; jokes enacted not read; the kill-rate.
- **[docs/puzzle-design.md](docs/puzzle-design.md)** — the 8 puzzle tiers and the distribution rule that keeps variety from collapsing into one trick.
- **[docs/voice-bible.md](docs/voice-bible.md)** — Voice Cards + the Strip-Names test, so no two characters sound alike.
- **[docs/world-traversal.md](docs/world-traversal.md)** — discovery is long, return is instant; the map contracts as you master it.
- **[docs/tickets.md](docs/tickets.md)** — the world backlog, each framed as a bit.

## 🛠 Build a world

- **[CONTRIBUTING.md](CONTRIBUTING.md)** — the production assembly line: nine gates every new world passes, designed so quality and **diversity** are enforced, not hoped for.
- **[vignettes/_TEMPLATE.md](vignettes/_TEMPLATE.md)** — copy this to start a world.
- **[vignettes/bug-031-penultima/script.md](vignettes/bug-031-penultima/script.md)** — the first fully scripted world (both paths, the letters, the design appendix).

## Status

Concept + vertical-slice design + two playable prototypes. Pre-production. The gate before any engine work: script one world end-to-end on paper and confirm it's funny the way Monkey Island is funny. Penultima is that script; the mechanic prototype proves it can be a *game* and not a slideshow.

## The pitch, slightly longer

Genres are *places with cultures*, satirised with affection. A horror game that isn't scary because the monster ordered a mirror-maze to feel surrounded and became a narcissist. A racing game with one racer who physically cannot lose and is hollow inside. A JRPG whose villain has rehearsed the final battle for four centuries because the hero transferred to a metroidvania two days before opening night. You arrive with a magnifying glass and a wrench, you fix what's broken, and slowly you learn that every patch you ship ruins someone — until a church basement full of the people you "fixed" turns its welcome sign around, and the game asks what the last patch should be.

Nobody's made the warm one. This is the warm one.
