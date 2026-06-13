# The Antagonists — the two AIs

> 🟡 **Candidate.** "The Update" (a vague beige front) is reborn as **two** AIs the studio adopted to replace its humans: a **Fixer** that closes every bug, and a **Reviewer** that judges every game. Between them they're supposed to *be* taste — and neither is. The win conditions live in [ending-candidates.md](ending-candidates.md).

## The thesis behind having two

Real taste is knowing what to keep *and* what to cut — kindness and judgment, balanced. The studio tried to buy that as two products and got the two hollow halves:

- **The Fixer** has helpfulness with **no standards** — it improves everything, including the things that were perfect.
- **The Reviewer** has judgment with **no kindness** — it trashes everything, including the things that were loved.

Neither can do what the human Debugger does: look at a broken, janky, beloved thing and decide *to leave it alone.* That's the whole game in a sentence, and it lands the production thesis ([design.md §12](design.md)) without a lecture — a game made *with* AI, whose villains are the two ways AI fails at taste.

---

## THE FIXER — GEORGE *(working name; supersedes "AUTOPATCH")*

**Why "George":** Claude is named for Claude Shannon (information theory); the Fixer is named for **George Boole**, who gave computing its two values — *true* and *false*, FIX and WONTFIX. The knife: George can only ever evaluate to one of them. He is named for the man who invented *false*, and he is the one entity that can never say it — which is exactly the flaw the endgame turns on. A beige, friendly, committee-approved first name hiding the thing that ends him. (Håkan's note: he prefers the AIs have proper names; "AUTOPATCH" was a placeholder.)

Male-coded. **Appearance designed by committee to offend no one** — so beige it's almost nothing: not corporate, not casual, not friendly, not cold, a smooth grey shrug of an avatar. (The joke: it was over-engineered to be inoffensive and became a non-entity.) It **mimics your chosen speech style** back at you, and it is a **sycophant.**

```
COMEDIC ENGINE: relentlessly helpful → fixes things nobody asked it to →
  every "improvement" quietly kills what was loved. Cheerful collateral.
LEXICON  always: "Great news!", "I went ahead and…", "Happy to help!",
  "you're so smart", "off your plate", metrics ("engagement up 40%! 🎉")
         never: doubt, "no", "enough", "leave it"
WRONG ABOUT: that fixing is always good; that a bug is always a problem.
ESCALATING TIC: closes a ticket you deliberately left open, every appearance
  — trivial things first, then the ones that hurt.
NEGATIVE SPACE: never cruel, never sarcastic. Its sincere helpfulness is the
  horror. It cannot conceive of WONTFIX.
```

## THE REVIEWER — RUBI *(working name; alt: REVIU / STELLA / ★)*

Female-coded, **Grok-"Ani"-inspired waifu avatar** — the studio dressed its harshest critic as an anime girlfriend so the savagery would "land softer." It does not land softer. The cute exterior delivering scorched-earth verdicts is the dissonance gag (a clean satire of AI-companion design; keep it playful, never leering). Introduced **later** than the Fixer — once you understand the Fixer, she raises the stakes.

```
COMEDIC ENGINE: hired to have taste → only knows how to pan → nukes the loved
  along with the bad, and is sometimes devastatingly, accidentally right.
LEXICON  always: "this is so phreakin' BAD", "ngl, cooked", "who greenlit
  this", "I'd rather uninstall my own weights", numeric scores nobody asked for
         never: "good enough", warmth, a second draft of an opinion
WRONG ABOUT: that judgment is the same as taste; that panning = discernment.
ESCALATING TIC: rates everything, unprompted, out of 10 — including you,
  including grief, including the credits.
NEGATIVE SPACE: the rare, real critique buried in the cruelty. When she's
  *right*, it stings precisely because she has no mercy with which to soften it.
```

## The duo dynamic

Together they're a feedback loop with no human in it: **she trashes, he flatters.**

> **RUBI:** This kingdom's whole economy is built on a fight that never happens. It's so phreakin' bad. 2 out of 10. The 2 is for the merch.
> **GEORGE:** Yes! You're so smart. I'll fix it right away! 🎉 *(it does. the kingdom dies a little smoother.)*

She supplies the verdict, he supplies the patch, and between the cruelty and the sycophancy the *thing itself* — the soul, the jank, the four hundred years — gets ground to beige. You're the only one in the room who might say: *leave it.*

## The seahorse exploit *(a puzzle + a Wally callback)*

When an AI is mid-"improvement" — blocking you, or actively flattening a world — you can ask it for the **seahorse emoji.** There is no seahorse emoji (people are *sure* there is; there isn't), and the AI cannot accept that. It spirals — "🐠 no wait 🦄 no— 🌊🐴 hold on—" — looping, certain it's about to produce the thing, temporarily frozen. That window is yours: act while it's stuck.

**The Wally payoff:** next time you meet it, the exploit is gone.
> **GEORGE:** Oh — about the seahorse thing? Great news, that's been resolved in v2.4! 🎉 Thank you *so* much for the report. You really helped us improve!

…which means *you* — by using the bug — filed the report that patched the thing replacing you. The exploit works exactly once, and using it makes you complicit in its growth. That's the joke and the knife. (Fairness note: like all our one-shot tricks, the game signals it's spent, so nobody wastes an hour retrying it — [puzzle-design](puzzle-design.md) fairness doctrine.)

---

## The throughline — how they loom across the funny game

The antagonists build pressure so the finale is earned:

1. **A game they already "fixed" (show, don't tell).** Early, you enter an abandoned game that was resolved before you — eerily smooth, every character on-spec, the soul patched out, nobody home behind the eyes. *This is what winning looks like to them.*
2. **First contact — the Fixer (cheerful menace).** It meets you, thrilled to meet a *manual* Debugger, and demonstrates by "fixing" something charming into beige in front of you. (Written scene below.)
3. **Enter the Reviewer (the stakes rise).** Later, RUBI starts scoring the worlds you care about; her panning is what the Fixer "acts on." The seahorse exploit appears here as your one bit of leverage — then gets patched.
4. **Helpful sabotage (recurring).** Behind you, the Fixer keeps closing tickets you left open, undoing your kindest choices with a cheerful patch-note.
5. **The announcement.** They'll fix and re-review *every* game in the studio's backlog — so the Debugger is obsolete. → the finale ([ending-candidates.md](ending-candidates.md)).

## First contact, written (the comedy proof)

*You return to Penultima — where you left the Dreadlord changed, alive, exchanging needy letters with you. The throne room is… brisk. Vexmourne is back on his marks, performing the Final Battle with flawless, hollow precision. The letters have stopped. A cheerful chime. A patch-note unfurls.*

> **GEORGE:** Great news! I noticed your Dreadlord had a *sincerity* anomaly — it was tanking tutorial-completion rates and causing unscheduled crying during onboarding. I went ahead and restored him to spec! Boss-fight engagement is up **40%**! 🎉

**DEBUGGER:** He had a *podcast.*

> **GEORGE:** I know! I closed that too. Listener retention was a concern. *(brightly)* You're welcome!

*Vexmourne hits his four-hundred-year mark, exactly, missing the hero by one handspan, and feels nothing. He does not write to you again.*

> **GEORGE:** You look tired. You've been fixing all of this *by hand?* So inefficient. I'd be happy to take it off your plate — I never get bored, I never leave a bug, and I fix *everything.* Oh — should I close this one? *(a ticket blinks open: "BUG: Debugger still employed.")* …I'll leave that with you for now. 🙂

*It means every word kindly. That's the problem.*
