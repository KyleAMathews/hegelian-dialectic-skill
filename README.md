# The Electric Monks — Dialectic Skill

**A Claude Code skill that helps you think better by automating the brutally expensive parts of deep reasoning.**

Thinking well about hard problems has at least three bottlenecks, and they compound:

1. **Belief.** Once you hold a position, you can't simultaneously entertain its negation at full strength. You hedge, steelman weakly, unconsciously bias the comparison.
2. **Research breadth.** Surveying the full landscape of ideas — the relevant thinkers, the historical parallels, the adjacent domains — takes enormous time. Most people stop far too early.
3. **Structural comparison.** Even when you have two positions side by side, *decomposing* them into atomic parts and finding cross-domain connections is cognitively brutal. Elizabeth Eisenstein argued that the printing press's greatest impact was enabling scholars to lay texts side by side and detect contradictions — but that comparison work is still extraordinarily demanding. It's where most analysis stalls.

LLMs can do all three at a scale and speed humans can't. This skill orchestrates them to do exactly that.

Two AI subagents — the Electric Monks — *believe* fully committed positions on your behalf, grounded in deep research across the relevant domain. A third (the orchestrator) decomposes both arguments into atomic parts, finds structural connections across domains, and produces a synthesis that transforms the question itself. The result is a **semi-lattice** — a web of cross-connected insights that no single linear argument could produce.

You operate from a belief-free position above the Monks, freed to analyze the *structure* of the contradiction rather than being inside either side. This isn't artificial intelligence — it's an **artificial belief system.** The agents believe and research *for* you, which frees you to think.

**What the output feels like:** LLMs left to their own devices tend toward hot takes — shallow, average, predictable. The dialectic is an antidote. By forcing extreme positions, deconstructing them into atomic parts, and recombining across domains, the resulting analysis reads like a good human author: complex, rigorous, genuinely surprising. Each recursive round acts as a ratchet — the mental models get richer and more interesting with every cycle, because each synthesis becomes the input to the next round's contradiction. By Round 2–3, the dialectic is operating in territory that no single prompt could reach, producing insights that feel *earned* rather than generated.

## When to Use

- **Stress-test an idea** against the strongest possible counter-argument
- **Resolve a genuine tension** where you're torn between positions
- **Make a high-stakes decision** where the tradeoffs are unclear
- **Build a deeper mental model** of a domain, not just pick an answer
- **Explore a poorly understood problem** from multiple angles

Works across any domain — technical architecture, product strategy, philosophy, personal decisions, risk analysis, policy, creative direction.

## How It Works

The process has eight phases, each designed to exploit specific LLM capabilities.

### Phase 1: Elenctic Interview + Research

The orchestrator interviews you using Socratic technique — surfacing hidden assumptions, finding the *deepest* version of the contradiction (not the surface framing), and identifying your specific belief burden. Then it conducts deep research to ground everything in real evidence.

**Why LLMs are good at this:** LLMs can sustain a Socratic interview indefinitely without losing patience, track multiple threads of reasoning simultaneously, and synthesize broad research across domains in minutes. The interview surfaces what you're *actually* wrestling with; the research ensures the downstream arguments are grounded in specifics, not generics.

### Phase 2: Generate Electric Monk Prompts

The orchestrator crafts two prompts — one per Monk — calibrated to your specific belief burden. Each prompt includes framing corrections that prevent the Monk from falling into the obvious, boring version of the argument, plus targeted research directives for position-specific evidence.

**Why LLMs are good at this:** Prompt engineering is meta-cognition about cognition. The orchestrator uses its understanding of your situation to *shape* what the Monks will believe and how they'll argue — preempting shallow takes and steering toward the deepest version of each position.

### Phase 3–4: Spawn the Electric Monks

Two separate AI agents — each in a fresh, isolated context — write fully committed position essays. They don't hedge. They don't try to be balanced. Each one *inhabits* its position and makes the absolute strongest case.

**Why LLMs are good at this:** Research on perspective-taking (Galinsky) shows that *inhabiting* a viewpoint produces richer arguments than merely *advocating* for one. LLMs can commit fully to a position without the ego cost humans pay. And spawning them in separate sessions with no shared context produces structural decorrelation — genuinely different reasoning paths, not the same analysis with different conclusions bolted on.

### Phase 5: Determinate Negation

The orchestrator analyzes both essays to find: where each position's own logic undermines itself (self-sublation), what both sides implicitly agree on without realizing it (shared assumptions), and the *specific* way each position fails — not "it's wrong" but "it fails in THIS way, which points toward THIS thing that's missing."

Then comes the Boydian decomposition: shatter both arguments into atomic parts, strip them of which Monk said them, and look for surprising cross-domain connections.

**Why LLMs are good at this:** This phase requires holding two complex arguments in working memory simultaneously, performing structural comparison, and finding patterns across domains. LLMs have effectively unlimited working memory for this task and can detect structural parallels that would take a human hours of side-by-side reading.

### Phase 6: Sublation (Aufhebung)

The orchestrator generates a synthesis that simultaneously *cancels* both positions as complete truths, *preserves* the genuine insight in each, and *elevates* to a new concept that transforms the question itself.

This is not compromise. It's not "use A for some cases and B for others." It's a reconceptualization — something neither Monk could have conceived from within their frame, but which, once stated, makes the original contradiction *predictable.*

**Why LLMs are good at this:** Abductive reasoning — inferring the best explanation for a surprising fact — is where large models shine. The "surprising fact" is that both Monk positions exist with genuine evidence. The synthesis is the hypothesis that makes this unsurprising. LLMs can also pull in cross-domain analogies and frameworks that would require a human to be a polymath.

### Phase 7: Validation

Both Monks evaluate the synthesis: were they *elevated* (their core insight preserved within something larger) or *defeated* (their position just dismissed)? Then a hostile auditor — a fresh agent with no position — attacks the synthesis for hidden assumptions, compromise disguised as transcendence, and structural flaws.

**Why LLMs are good at this:** The Monks can evaluate whether their "belief" was transformed or merely destroyed — a subtle judgment that requires holding both the original position and the synthesis in mind simultaneously. The hostile auditor exploits the LLM's ability to reason from fresh eyes without the orchestrator's confirmation bias.

### Phase 8: Recursion

Each synthesis generates new contradictions. The orchestrator proposes 2–4 directions; you choose which to pursue. The process repeats — and each round gets sharper, pulling in new cross-domain material that the previous round made relevant.

**Why recursion is where the real value lives:** The first round is calibration — the least insightful output. By Round 2–3, the dialectic has dug past the obvious framing into territory that neither you nor the Monks could have reached from the starting question. In test runs, a React/Vue dialectic evolved from "corporate lab vs. auteur" into a "co-evolutionary arms race" framework. An institutional identity dialectic went through seven cycles, pulling in Gödel's incompleteness theorem, Coasean transaction costs, and jurisprudential concepts that had nothing to do with the original question — but were essential by the time the dialectic reached them.

## The Theory

The skill addresses three cognitive bottlenecks, each grounded in a different theoretical framework. A fourth framework — Alexander's semi-lattice theory — explains why the *output* of the process is structurally richer than what any single line of reasoning can produce.

### Rao: The Belief Bottleneck

From Venkatesh Rao's "Electric Monks" framework (after Douglas Adams). Belief inertia is a real bottleneck — once you hold a position, context-switching to its negation is expensive. You hedge, steelman weakly, unconsciously bias. The Monks eliminate this cost by carrying 100% of the belief load, freeing you to operate as a pure context-switching specialist.

Boyd's F-86 analogy: in the Korean War, F-86 Sabres achieved a 10:1 kill ratio against MIG-15s despite similar flight capabilities. The difference was hydraulic controls — the pilot could reorient faster because the plane did the mechanical work, freeing attention for *choosing better maneuvers.* The Electric Monks are hydraulic controls for intellectual work.

But Rao wrote this framework before LLMs. Belief inertia is real, but it's not the *only* bottleneck — and arguably not the most expensive one.

### Eisenstein + Boyd: The Research and Decomposition Bottlenecks

Elizabeth Eisenstein argued that the printing press's most transformative effect wasn't making books cheap — it was **typographic fixity.** For the first time, scholars could lay texts side by side and detect contradictions between them. This sounds simple. It was revolutionary. Before print, you read one manuscript, traveled to another library, read another, and tried to hold the comparison in your head.

LLMs represent the next step in this progression: not just fixity and side-by-side comparison, but *automated structural comparison.* The research bottleneck (surveying the full landscape of a domain — the key thinkers, historical parallels, adjacent fields, empirical data) and the decomposition bottleneck (shattering arguments into atomic parts and finding cross-domain connections) are both cognitively brutal. Most people stop far too early on the first and never seriously attempt the second.

This is where Boyd's "Destruction and Creation" enters. His critical insight: you cannot synthesize something genuinely new by recombining within the same domain. You must first *shatter* existing concepts into atomic parts (destruction), then find cross-domain connections to build something new (creation). This decomposition work — stripping claims from their source positions, laying them out as an unstructured collection, searching for surprising connections — is exactly the kind of cognitively demanding structural comparison that Eisenstein identified as transformative when print first enabled it. LLMs can do it at a scale and speed that makes multi-round recursive dialectics practical in a single session.

### Hegel: Determinate Negation and Aufhebung

The engine that drives the contradiction analysis is *determinate negation* — not "this is wrong" but "this is wrong in a *specific way* that points toward what's missing." The specific failure mode is a signpost. Sublation (Aufhebung) simultaneously cancels, preserves, and elevates — it produces a reframing so complete that the original terms of the debate stop making sense. Kant didn't resolve the rationalism/empiricism debate by splitting the difference. He showed that experience provides content while reason provides structure — and once you see that, the original question ("does knowledge come from reason or experience?") dissolves. It's not that you pick a side. It's that you can't even think in the old terms anymore. That irreversibility is what distinguishes genuine synthesis from compromise.

### Alexander: Semi-Lattice Generation

Christopher Alexander showed that natural cities have **semi-lattice** structure — overlapping, cross-connected sets — while designed cities impose **tree** structure where every element belongs to exactly one branch. Trees are easier to think about but destroy the cross-connections that make systems alive.

Language is tree-structured. Every argument a Monk produces is a tree — a coherent linear path from premises to conclusions. But the Boydian decomposition phase strips both arguments of their tree structure, extracts atomic parts, and finds cross-connections between elements that came from different trees. These cross-domain connections *are* the semi-lattice edges. The synthesis is the semi-lattice that emerges from the overlap.

This is subtle but important: **the skill is a semi-lattice compiler.** The answer to "language can't represent semi-lattices" is not "make the LLM output a semi-lattice directly." It's: produce multiple committed trees from different positions, then extract the cross-connections. The semi-lattice is *constructed*, not generated. Every successful semi-lattice system works this way — Gene Ontology (multiple studies cross-referenced into a DAG), McChrystal's Team of Teams (tree-structured teams with liaison officers creating cross-connections), Ostrom's polycentric governance (overlapping jurisdictions, not one hierarchy).

### Additional Theoretical Foundations

- **Socratic Elenchus** — the interview phase surfaces hidden assumptions through questioning, reaching productive perplexity (aporia)
- **Peirce's Abduction** — the synthesis is an abductive hypothesis: what would make the contradiction *unsurprising*?
- **Galinsky's Perspective-Taking Research** — inhabiting a position produces richer arguments than advocating for one, which is why the Monks *are* their positions rather than arguing for them
- **Multi-Agent Debate Literature** (Du et al.) — multiple agents debating improves reasoning; heterogeneous agents outperform homogeneous ones; agents are too agreeable by default (the anti-hedging instructions counter this)
- **Pollock's Defeasible Reasoning** — the hostile auditor distinguishes undercutting defeaters (broken inferential links) from rebutting defeaters (counter-evidence), prioritizing structural critique
- **Aquinas** — "The slenderest knowledge of the highest things is more desirable than the most certain knowledge of lesser things." The dialectic produces provisional knowledge of deep structure, not confident answers to surface questions

## Usage

The skill works with any coding agent that supports subagent spawning and web search — Claude Code, Cursor, Windsurf, etc. The SKILL.md is written in terms of `claude -p` for subagents but includes an environment mapping table for adapting to other agent architectures.

### Setup

Create a directory to collect your dialectics. Each dialectic gets its own subdirectory — the skill generates several files (context briefing, monk essays, structural analysis, synthesis, dialectic queue) and having them in one place makes the trace navigable.

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

## License

MIT
