# Missing Heritability and the Smuggled Gene

## STUDY

The persistent gap between heritability estimated from twin studies and heritability explained by identified genetic variants (GWAS). For most complex traits, twin studies suggest 40–80% heritability, while GWAS collectively explain 10–30%. This "missing heritability" has driven massive investment in whole-genome sequencing, rare variant analysis, and expanded cohort studies.

Key ongoing efforts: UK Biobank (500,000 participants, whole-genome sequencing ongoing), All of Us (NIH, targeting 1 million participants), and large-scale whole-exome sequencing studies. Results are published continuously throughout 2026.

Critical recent finding: Nature November 2025 — "Specificity, length and luck drive gene rankings in association studies" — demonstrated that GWAS and rare-variant burden tests systematically prioritise *completely different genes for the same traits*. GWAS prioritise genes near trait-specific non-coding variants; burden tests prioritise trait-specific coding genes. The sets barely overlap.

## CONSENSUS EXPECTATION

The field expects the gap to close as sample sizes increase and analytical methods improve. The standard narrative: missing heritability is hiding in rare variants (too infrequent for earlier studies to detect), structural variants (poorly captured by SNP arrays), gene-gene interactions (statistically underpowered), and gene-environment interactions (not yet modelled). With whole-genome sequencing and million-person cohorts, the gap should narrow substantially.

The consensus timeline: each major data release explains a few more percentage points. By 2030, the gap will be substantially closed.

Our prediction directly contradicts this timeline and partially contradicts the framing.

## PREDICTION

1. **UK Biobank whole-genome sequencing results (2026) will identify additional variants but will not substantially close the heritability gap.** The pattern already established will continue: each new tranche of data adds more variants, each explaining less variance individually, with diminishing marginal returns. For well-studied traits (height, BMI, schizophrenia), GWAS-explained heritability will remain below 40% of twin-study estimates using additive models, even with whole-genome data from 500,000+ individuals.

2. **The Nature 2025 finding — GWAS and burden tests prioritise different genes — will replicate across traits and datasets.** This is the smuggling signature: the method of looking determines what you find, meaning "a gene's contribution" is not a property of the gene but a joint property of the gene, the analytical method, and the context.

3. **Gene-gene interaction studies, enabled by larger cohorts and more compute, will find that interactions are pervasive but explain less additional variance than expected.** This is because interactions are not an additive correction to a fundamentally additive system — they are the primary mode of genetic causation. When you find them, they don't slot into the additive framework as "extra variance explained"; they reveal that the additive framework was the wrong decomposition.

4. **Polygenic risk scores will plateau in predictive power well below twin-study heritability estimates**, even with complete genome sequences and optimal statistical methods. The plateau will be interpreted as evidence that "environment" must explain the rest, which will not be satisfying either, because twin studies already account for shared environment. (Note: PRS limitations are increasingly acknowledged within genetics. This prediction aligns with growing scepticism. What differs is the explanation: the consensus attributes the plateau to missing data or inadequate models. We attribute it to the additive decomposition being structurally wrong — a distinction with different implications for what would fix it.)

## STRUCTURAL REASONING

This is a smuggling error. The question "which genes contribute to this trait, and how much?" smuggles in a concept — the independently quantifiable contribution of a single gene — that was never established and doesn't correspond to how genomes work.

Twin studies measure the total effect of shared DNA. GWAS attempt to decompose this total effect into individual variant contributions. The decomposition assumes that genetic causation is additive: variant A contributes X%, variant B contributes Y%, and you can sum them. This is the smuggled premise. It was never derived from genetics — it was imported from statistical methodology (linear regression) and treated as a biological claim.

The genome doesn't work additively. Gene expression is context-dependent (which variants are present at other loci, which tissues are active, which environmental signals are present). The "contribution" of a variant is not a property of the variant — it is a property of the variant-in-context, and the context includes the rest of the genome and the environment. Asking "how much does this variant contribute?" is like asking "how much does this word contribute to this sentence?" — the question has a formal answer in an information-theoretic framework but that answer doesn't capture how meaning works.

The missing heritability isn't hiding. It was never the kind of thing that could be found by summing individual contributions, because the individual contributions don't exist independently. This is orthogonal to the stated question — the field is looking for more variants, when the problem is in the concept of "a variant's contribution."

## WHAT WOULD DISCONFIRM THIS

- Whole-genome sequencing closes the heritability gap to within 10% for multiple complex traits (height, BMI, schizophrenia) using additive models. This would mean the additive decomposition works — the missing variants were just rare.
- A gene-gene interaction model explains ≥20% additional variance beyond additive models for a major complex trait, in a way that adds cleanly to the additive estimate. This would mean interactions are a correction to an additive base, not a different mode of causation.
- Polygenic risk scores from complete genome data achieve predictive accuracy matching twin-study heritability estimates. This would mean the decomposition does capture total genetic effects.

## DOMAIN

genetics

## DATE

2026-03-08
