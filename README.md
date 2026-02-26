# The Electric Monks — Dialectic Skill

*Named after Douglas Adams' machines built to believe things for you*

**An agent skill that helps you think better by automating the brutally expensive parts of deep reasoning.**

Two AI subagents — the Electric Monks — *believe* fully committed positions on your behalf. A third, the orchestrator, decomposes both arguments into atomic parts, finds cross-domain connections, and synthesizes. The result is a **semi-lattice** — a structure no single linear argument could produce.

You operate from a belief-free position above the Monks, analyzing the *structure* of the contradiction rather than being inside either side. This isn't artificial intelligence — it's an **artificial belief system** that frees you to think.

**What the output feels like:** Left alone, LLMs produce shallow takes. The dialectic breaks that pattern. As you read through the Monks' committed arguments, connections come to mind — things neither side considered, corrections to their framing, ideas you hadn't articulated yet. You feed these back in. The skill tunes to your thinking more and more with each round, but it also rigorously exposes the contradictions in that thinking — so you get an increasingly full and precise map of your own ideas. Then the skill breaks it apart and reforms it as something richer and more interesting than what you started with. Each synthesis becomes the next round's thesis, and by Round 2–3 the dialectic is operating in territory no single prompt could reach.

**Why this works** — thinking well about hard problems has at least three bottlenecks, and they compound:

1. **Belief.** Once you hold a position, you can't simultaneously entertain its negation at full strength. You hedge, steelman weakly, unconsciously bias the comparison.
2. **Research breadth.** Surveying a domain's thinkers, history, and adjacent fields takes enormous time. Most people stop too early.
3. **Structural comparison.** Even with two positions side by side, decomposing them into atomic parts and finding cross-domain connections is cognitively brutal. Most analysis stalls here.

LLMs can do all three at a scale and speed humans can't. This skill orchestrates them to do exactly that.

## When to Use

- **You've locked onto a vision and can't genuinely entertain alternatives.** You have a strong thesis — maybe an architecture, a strategy, a life direction — and you want to stress-test it, but you keep steelmanning the other side weakly.
- **You're trying to do everything because cutting anything feels like betrayal.** Competing needs all feel equally urgent. You can't triage because every priority has someone counting on it.
- **You can argue every side but can't commit to any of them.** You find the question intellectually interesting but "what do *you* actually think?" produces discomfort. You've explored this before without resolution.
- **You've optimized a system and suspect you might be optimizing the wrong thing.** Your approach works — you have data to prove it — but the landscape may have shifted and you can't see past your own competence.
- **Your own values contradict each other.** You believe multiple things passionately, each feels individually right, but collectively they're impossible. The tension is internal, not external.
- **"This is how it's done" has become invisible as an assumption.** You have deep knowledge of how things work, but you suspect it's blinding you to radically different approaches.

Works across domains — technical architecture, product strategy, philosophy, personal decisions.

## Usage

The skill works with any coding agent that supports subagent spawning and web search — Claude Code, Cursor, Windsurf, etc.

**This is a heavy process by design.** Expect 10–15 minutes per round minimum, and plan for at least 3 rounds. This skill needs the best available model — every phase benefits from maximum reasoning capability.

### Setup

Create a directory to collect your dialectics. Each dialectic gets its own subdirectory — the skill generates several files (context briefing, monk essays, structural analysis, synthesis, dialectic queue).

```
dialectics/
├── tanstack-vs-nextjs/
│   ├── context_briefing.md
│   ├── monk_a_output.md
│   ├── monk_b_output.md
│   ├── determinate_negation.md
│   ├── sublation.md
│   └── dialectic_queue.md
├── agent-governance/
│   └── ...
└── career-decision/
    └── ...
```

### Running a Dialectic

1. Create a subdirectory for your topic:
   ```bash
   mkdir -p ~/dialectics/my-topic && cd ~/dialectics/my-topic
   ```

2. Start your coding agent in that directory. In Claude Code:
   ```bash
   claude
   ```

3. Load the skill and give it your question:
   ```
   /install-skill /path/to/SKILL.md

   I want to explore: [your topic or tension here]
   ```

   The skill will walk you through the elenctic interview, spawn the Monks, and produce the full dialectical trace — all saved as files in the current directory.

### Tips

- **You are the co-pilot.** Interrupt, correct, redirect at any point. The Monks will get things wrong. Your corrections are the highest-leverage input in the entire process.
- **The first round is calibration.** Don't judge the skill by Round 1. The real insights come in Rounds 2–3, once the process has dug past the obvious framing.
- **Say yes to recursion.** When the skill proposes recursive directions after a synthesis, pick one. Each round ratchets up the quality.
- **The dialectic queue persists.** The `dialectic_queue.md` file tracks explored and unexplored contradictions. You can come back to it in a future session and pick up where you left off.

## How It Works

The process has seven phases.

### Phase 1: Elenctic Interview + Research — surface the real contradiction

The orchestrator interviews you Socratically — surfacing hidden assumptions, finding the deepest version of the contradiction, and identifying your belief burden. Then it researches the domain to ground both sides in specifics. The interview surfaces what you're *actually* wrestling with; the research ensures the downstream arguments are grounded in specifics, not generics.

### Phase 2: Generate Electric Monk Prompts — calibrate the belief assignments

The orchestrator crafts two prompts — one per Monk — calibrated to your specific belief burden. Each prompt includes framing corrections that prevent the Monk from falling into the obvious, boring version of the argument, plus targeted research directives for position-specific evidence.

### Phase 3: Spawn the Electric Monks — two fully committed position essays

Two separate AI agents — each in a fresh, isolated context — write fully committed position essays. They don't hedge. They don't try to be balanced. Each one *inhabits* its position and makes the absolute strongest case. Spawning them in separate sessions with no shared context produces structural decorrelation — genuinely different reasoning paths, not the same analysis with different conclusions bolted on.

### Phase 4: Determinate Negation — find where each argument undermines itself

The orchestrator analyzes both essays to find: where each position's own logic undermines itself (self-sublation), what both sides implicitly agree on without realizing it (shared assumptions), and the *specific* way each position fails — not "it's wrong" but "it fails in THIS way, which points toward THIS thing that's missing."

Then comes the Boydian decomposition: shatter both arguments into atomic parts, strip them of which Monk said them, and look for surprising cross-domain connections.

### Phase 5: Sublation (Aufhebung) — synthesize something neither side could reach

The orchestrator generates a synthesis that simultaneously *cancels* both positions as complete truths, *preserves* the genuine insight in each, and *elevates* to a new concept that transforms the question itself.

This is not compromise. It's not "use A for some cases and B for others." It's a reconceptualization — something neither Monk could have conceived from within their frame, but which, once stated, makes the original contradiction *predictable.* The synthesis is an abductive hypothesis: what would make it *unsurprising* that both Monk positions exist with genuine evidence?

### Phase 6: Validation — did the Monks feel elevated or defeated?

Both Monks evaluate the synthesis: were they *elevated* (their core insight preserved within something larger) or *defeated* (their position just dismissed)? Then a hostile auditor — a fresh agent with no position — attacks the synthesis for hidden assumptions, compromise disguised as transcendence, and structural flaws.

### Phase 7: Recursion — where the real value lives

Each synthesis generates new contradictions. The orchestrator proposes 2–4 directions; you choose which to pursue. The process repeats — and each round gets sharper, pulling in new cross-domain material that the previous round made relevant.

The first round is calibration — the least insightful output. By Round 2–3, the dialectic has dug past the obvious framing into territory that neither you nor the Monks could have reached from the starting question. In test runs, a React/Vue dialectic evolved from "corporate lab vs. auteur" into a "co-evolutionary arms race" framework. An institutional identity dialectic went through seven cycles, pulling in Gödel's incompleteness theorem, Coasean transaction costs, and jurisprudential concepts that had nothing to do with the original question — but were essential by the time the dialectic reached them.

## The Theory

The skill rests on three theoretical frameworks — one per bottleneck — plus Alexander's semi-lattice theory, which explains why the output is structurally richer than any single line of reasoning.

### Rao: The Belief Bottleneck

From Venkatesh Rao's "Electric Monks" framework (after Douglas Adams). Belief inertia — the cost of genuinely entertaining a position's negation — is the bottleneck Rao identified. The Monks eliminate it by carrying 100% of the belief load, freeing you to operate as a pure context-switching specialist.

Boyd's analogy: in the Korean War, F-86 Sabres achieved a 10:1 kill ratio against MIG-15s despite similar flight capabilities. The difference was hydraulic controls — the pilot could reorient faster because the plane did the mechanical work, freeing attention for *choosing better maneuvers.* The Monks are hydraulic controls for intellectual work.

Rao wrote this framework before LLMs. Belief inertia is real, but it's not the only bottleneck — and arguably not the most expensive one.

### Eisenstein + Boyd: The Research and Decomposition Bottlenecks

Elizabeth Eisenstein argued that the printing press's most transformative effect wasn't making books cheap — it was **typographic fixity.** For the first time, scholars could lay texts side by side and detect contradictions. Before print, you read one manuscript, traveled to another library, read another, and tried to hold the comparison in your head.

LLMs represent the next step: not just fixity and side-by-side comparison, but *automated structural comparison.* Both remaining bottlenecks — research breadth and structural decomposition — are cognitively brutal. Most people abandon the first too early and never attempt the second.

This is where Boyd's "Destruction and Creation" enters. His critical insight: you cannot synthesize something genuinely new by recombining within the same domain. You must first *shatter* existing concepts into atomic parts (destruction), then find cross-domain connections to build something new (creation). This decomposition work — stripping claims from their source, searching for surprising connections — is the structural comparison Eisenstein identified as transformative when print first enabled it. LLMs can do it at a scale and speed that makes multi-round recursive dialectics practical in a single session.

### Hegel: Determinate Negation and Aufhebung

*Determinate negation* doesn't say "this is wrong." It says "this is wrong in a *specific way* that points toward what's missing." The failure mode is a signpost. Sublation (Aufhebung) simultaneously cancels, preserves, and elevates — it produces a reframing so complete that the original terms of the debate stop making sense. Kant didn't resolve the rationalism/empiricism debate by splitting the difference. He showed that experience provides content while reason provides structure — and once you see that, the original question ("does knowledge come from reason or experience?") dissolves. It's not that you pick a side. It's that you can't even think in the old terms anymore. That irreversibility is what distinguishes genuine synthesis from compromise.

### Alexander: Semi-Lattice Generation

Christopher Alexander showed that natural cities have **semi-lattice** structure — overlapping, cross-connected sets — while designed cities impose **tree** structure where every element belongs to exactly one branch. Trees are easier to think about but destroy the cross-connections that make systems alive.

Language is tree-structured. Every argument a Monk produces is a tree — a coherent linear path from premises to conclusions. But the Boydian decomposition phase strips both arguments of their tree structure, extracts atomic parts, and finds cross-connections between elements that came from different trees. These cross-domain connections *are* the semi-lattice edges. The synthesis is the semi-lattice that emerges from the overlap.

**The skill is a semi-lattice compiler.** The answer to "language can't represent semi-lattices" is not "make the LLM output a semi-lattice directly." It's: produce multiple committed trees from different positions, then extract the cross-connections. The semi-lattice is *constructed*, not generated. Every successful semi-lattice system works this way — Gene Ontology (multiple studies cross-referenced into a DAG), McChrystal's Team of Teams (tree-structured teams with liaison officers creating cross-connections), Ostrom's polycentric governance (overlapping jurisdictions, not one hierarchy).

### Additional Theoretical Foundations

- **Socratic Elenchus** — the interview phase surfaces hidden assumptions through questioning, reaching productive perplexity (aporia)
- **Peirce's Abduction** — the synthesis is an abductive hypothesis: what would make the contradiction *unsurprising*?
- **Galinsky's Perspective-Taking Research** — inhabiting a position produces richer arguments than advocating for one, which is why the Monks *are* their positions rather than arguing for them
- **Multi-Agent Debate Literature** (Du et al.) — multiple agents debating improves reasoning; heterogeneous agents outperform homogeneous ones; agents are too agreeable by default (the anti-hedging instructions counter this)
- **Pollock's Defeasible Reasoning** — the hostile auditor distinguishes undercutting defeaters (broken inferential links) from rebutting defeaters (counter-evidence), prioritizing structural critique
- **Aquinas** — "The slenderest knowledge of the highest things is more desirable than the most certain knowledge of lesser things." The dialectic produces provisional knowledge of deep structure, not confident answers to surface questions

## License

MIT
