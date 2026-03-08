# AI Benchmark Reflexivity

## STUDY

The accelerating cycle of AI benchmark creation, saturation, and replacement. Key data points:

- MMLU (2021): GPT-3 scored ~35%. By 2024, frontier models exceeded 90%. By 2026, saturated above 99% for all frontier models.
- GSM8K (2021): now saturated with contamination-adjusted accuracy drops of up to 13%.
- HLE (Humanity's Last Exam, Nature January 2026): 2,500 expert-level questions. Claude Opus 4.6 leads at 53.1% with tools. Designed to resist saturation.
- GDPval (2026): real-world economic task evaluation. Top model scores 70.9% on well-specified tasks.
- Artificial Analysis overhauled its Intelligence Index in January 2026, specifically because previous benchmarks had saturated. New index deliberately recalibrated so top models score ~50 instead of ~73.

Anti-contamination measures now standard: canary strings, temporal splits, dynamic benchmarks. Interactive Benchmarks proposed at ICLR 2026 as a new paradigm.

Benchmark half-life is shortening: GLUE saturated in ~18 months, SuperGLUE in ~18 months, MMLU in ~3 years, but GSM8K in ~2 years. HLE's trajectory will be the test case.

## CONSENSUS EXPECTATION

The field is split between two camps. **Optimists** believe harder benchmarks (HLE, GPQA-Diamond, FrontierMath) will maintain discriminative power by raising the difficulty ceiling. **Pessimists** believe benchmark saturation reflects genuine rapid capability growth and that saturation is a success signal, not a measurement problem.

Both camps share one assumption: that the solution to benchmark saturation is *better benchmarks* — harder questions, more robust anti-contamination measures, dynamic evaluation, human-in-the-loop scoring. The consensus is that saturation is an engineering problem.

Our prediction rejects this shared assumption.

## PREDICTION

1. **HLE will follow the same saturation trajectory as its predecessors**, reaching ≥80% for frontier models within 18–24 months of publication (by mid-2027 to early 2028). Anti-contamination measures will slow but not prevent this.

2. **The mechanism will not be primarily contamination or memorisation.** Models will achieve high HLE scores through generalised capabilities (tool use, chain-of-thought reasoning, retrieval-augmented generation) that are developed *because* HLE-like evaluations incentivise them. The benchmark's existence shapes the capability landscape it purports to neutrally measure.

3. **Each replacement benchmark will saturate faster than its predecessor.** The pattern: GLUE (~18mo) → SuperGLUE (~18mo) → MMLU (~36mo) → GSM8K (~24mo) → HLE (prediction: ~18–24mo). Despite benchmarks getting harder, the time-to-saturation will not increase proportionally because the development ecosystem increasingly optimises against the evaluation ecosystem.

4. **Interactive/agentic benchmarks will resist saturation longer but will face a different version of the same problem**: the evaluation framework becomes a training signal. Labs will develop agents specifically for the interactive evaluation paradigm, producing high scores that don't transfer to genuinely novel interactive contexts.

5. **No static or semi-static benchmark created before 2028 will maintain discriminative power among frontier models for more than 24 months.** This includes benchmarks specifically designed to resist saturation.

## STRUCTURAL REASONING

This is a Section 1 error: the description is not separate from what it describes.

A sceptic will note that this is Goodhart's Law: "when a measure becomes a target, it ceases to be a good measure." That's correct — Goodhart's Law is a specific instance of the Section 1 constraint. What the structural reasoning adds is the claim that this is not fixable by better engineering. Goodhart's Law is typically treated as a practical problem: design better metrics, use multiple metrics, keep metrics partially secret. Section 1 says the problem is structural: any public, standardised description of capability will become part of the environment shaping capability. You can slow the feedback loop. You cannot break it without making the description non-public or non-standardised, which defeats its purpose as a benchmark.

A benchmark is a description of capability. When published, it becomes part of the environment that shapes capability development. Training pipelines incorporate benchmark-like tasks. Researchers optimise architectures and training procedures against evaluation criteria. The benchmark's categories and difficulty gradients become attractors for development effort. The description changes what it describes.

This is not a practical problem solvable by better benchmark design. It is a structural constraint identified by Section 1 of the Axioms: you cannot coherently establish a gap between the description (the benchmark) and the thing described (the capability). Any measure of capability that is public and standardised will become a target, and becoming a target changes the capability landscape, which changes what the measure captures.

Anti-contamination measures address data leakage — a specific mechanism. But the reflexivity operates at a higher level: not "the model memorised the test answers" but "the existence of the test shaped the development of capabilities that happen to solve the test." You can prevent the first. You cannot prevent the second without keeping the benchmark secret, which prevents it from being a *standard* — defeating its purpose.

The shortening half-life is the empirical signature: as the AI development ecosystem becomes more responsive to evaluation signals, the feedback loop tightens and benchmarks saturate faster.

## WHAT WOULD DISCONFIRM THIS

- HLE maintains discriminative power (top model <70%, significant spread among frontier models) for ≥30 months without revision. This would mean the difficulty ceiling can outrun the optimisation loop.
- A benchmark design methodology is developed that demonstrably resists saturation for ≥3 years across multiple model generations, without relying on secrecy. This would mean the Section 1 constraint can be engineered around.
- Saturation half-life increases rather than decreases for benchmarks published after 2026. This would mean the reflexivity loop is weakening rather than tightening.

## DOMAIN

artificial-intelligence

## DATE

2026-03-08
