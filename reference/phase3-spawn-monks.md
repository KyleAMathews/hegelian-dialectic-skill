# Phase 3: Spawn the Electric Monks

Spawn Monk A and Monk B as separate subagent sessions. Use `claude -p` (or your environment's equivalent for spawning an independent agent) so each gets a clean context with full belief commitment.

```bash
# Example for Claude Code:
echo "[MONK A PROMPT]" | claude -p --allowedTools web_search,web_fetch,read_file > monk_a_output.md
echo "[MONK B PROMPT]" | claude -p --allowedTools web_search,web_fetch,read_file > monk_b_output.md
```

These can run in parallel if your environment supports it.

**Efficiency note:** With the context briefing in place, monks need only 2-3 targeted searches each (vs. 15-25 without it). For personal/values domains, monks may need zero additional searches — the briefing contains the user's own material which is the primary evidence base.

**For recursive rounds (Phase 7):** See Phase 7 for guidance — recursive rounds may or may not need new research depending on whether the new contradiction opens new conceptual domains.

**After both complete:** Read both outputs carefully. Check:
- Did each monk actually *believe* fully, or did it hedge? (A hedging monk has failed its core function.)
- Did the framing corrections work, or did a monk fall into the degenerate framing?
- Are the arguments grounded in specific evidence (from the briefing or their own searches)?

**Decorrelation check:** Verify the monks actually diverged. The skill's value comes from *structurally uncorrelated* exploration of the problem space. Check:
- Do the monks cite *different* evidence, or substantially overlapping sources?
- Do they frame the problem using *different* conceptual vocabularies?
- Do their unstated assumptions *diverge*, or do they share the same background framework?
- Would a reader recognize these as genuinely *different perspectives,* or the same perspective with different conclusions bolted on?

If decorrelation is low — the monks are in "same framework, different conclusions" mode — consider reformulating the belief burdens to force genuinely different conceptual frames, not just different positions within one frame.

**If a monk's output hedges or is off-base:** Prefer restarting with a revised prompt over nudging. Fresh context with better instructions produces better results than correcting a monk that's lost its conviction.

**Present both outputs to the user** with a brief re-explanation of what they're looking at and what to do with it:

> Here are two essays — each one fully committed to one side of the tension we've been discussing. They're called "Electric Monks" because their job is to *believe* these positions so you don't have to. That frees you to read both and notice the *structure* of the disagreement from the outside.
>
> **A few important things as you read:**
> - **These will get things wrong.** The monks are working from what I told them, and I may have gotten your situation wrong, or they may have made assumptions that don't match your reality. That's expected — especially in this first round.
> - **Correct them freely.** If a monk says something that's off-base, tell me. "That's not how it works" or "they're missing that..." — these corrections are the most valuable input in the entire process. The synthesis can only be as good as the positions it's built on.
> - **The first round is the least insightful.** Think of it as calibration. Each subsequent round gets sharper, more specific, and more tuned to what you actually care about. The real breakthroughs usually come in rounds 2 and 3, once the process has dug past the obvious framing into the deeper tensions.
> - **Add anything that occurs to you.** New ideas, things neither monk mentioned, gut feelings you can't fully articulate — all of it is useful. You know your situation better than any of us.

Then ask:
1. Do these capture the positions accurately?
2. **"Is there a claim either monk makes that should be tested against evidence neither has considered?"** — This is the second high-leverage intervention point. In testing, users identified claims that sounded plausible but collapsed under scrutiny when tested against comparison classes the monks didn't consider. Catching this before synthesis prevents the entire downstream analysis from being built on an untested assumption.

If the user identifies a testable claim, run a targeted research agent to check it. This is cheap (~25-50K tokens) and can fundamentally change the quality of the synthesis.
