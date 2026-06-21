---
layout: page
title: Dimensional space of human emotions
description: Large-scale computational study of emotion experiences across narratives, videos, and real-life reports.
img: assets/img/emo_dim.png
importance: 1
category: work
related_publications: true
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/emo_dim.png" title="" class="img-fluid rounded z-depth-1 w-50" %}
    </div>
</div>
<div class="caption">
    Overview of the study {% cite han2024shared %}.
</div>

Emotions are ubiquitous and salient in human lives, and are a key feature of abnormal functioning in psychiatric disorders. One core debate regarding the structure of emotion experience can be roughly summarized as dimensional (typically proposes ‘‘core affect’’: valence and arousal, additional components can then be added to account for the full richness and diversity of human emotion experience) vs. categorical (e.g., classical basic emotion theory argues that emotions are best described by only a few basic emotions). We believe the debate is likely perpetuated by methodological constraints in previous work including the use of isolated stimulus sets, restricted rating scales, modest sample sizes, and inadequate analyses.

In this study, we did not set out to test any specific hypotheses or emotion theory. Instead, we were motivated by a strongly data-driven approach and aimed to be as comprehensive as possible and let the diversity of stimuli, ratings, and analyses speak for themselves.

<h2 style="font-size: 1.0rem; text-decoration: underline; font-weight: bold; margin-bottom: 0.5rem;">
1. Stimuli
</h2> 
We used three types of emotion-eliciting stimuli: **150 text narratives, 998 video clips and over 10,000 real-life experiences**. We performed **Principal Components Analysis (PCA)** on original ratings from previous studies to determine the number of narratives and videos needed to capture the majority of variance in the original sets. Final stimuli were selected via **maximum variation sampling**.	
<h2 style="font-size: 1.0rem; text-decoration: underline;  font-weight: bold; margin-bottom: 0.5rem;">
2. Scales
</h2> 
Our goal was to have a maximally diverse (but non-redundant) set of scales that describe the properties of emotion experiences.  We started by assembling **an inclusive list of 70 terms from literature**.  We then excluded those scales that described context rather than emotion, and combined synonymous and antonymous scales to eliminate redundancy to reduce the original set to 28 terms.

We verified that this refined set was **representative of the initial set** (Uniform Manifold Approximation and Projection (UMAP) applied to sentence embeddings of the scales), and relatively **high-dimensional in terms of their semantic meaning** and thus did not artificially constrain the dimensionality of the emotion experiences that they were used to rate (factor analysis applied to semantic similarity matrix among the 28 scales).

The quality of the scales were further assessed through **within-subject test-retest reliability (with Pearson correlations)** and **between-subject consensus (with split-half reliability)**.

<h2 style="font-size: 1.0rem; text-decoration: underline; font-weight: bold; margin-bottom: 0.5rem;">
3. Analyses
</h2> 
<h3 style="font-size: 1.0rem; text-decoration: underline; font-weight: bold; margin-bottom: 0.5rem;">
3.1 Dimensional Structure:
</h3> 
We first investigated whether the representational structure of emotion is consistent across stimulus domains and if it could be captured by a small number of interpretable dimensions.

We answered the first part using **Representational similarity analysis (RSA)**. We calculated the scale-by-scale Pearson correlation matrices for each stimulus type. High second-order Spearman rank correlations (second-order rs = 0.953, 0.923 and 0.909 for narratives and videos, narratives and real-life, and videos and real-life) confirmed that **the representational structure was highly consistent across stimulus types**.

Given the correlations across rating scales, we next used **Exploratory Factor Analysis (EFA)** to uncover the latent dimensions of emotion experiences. The number of factors (dimensions) to retain was determined using multiple criteria:

1. We used **statistical metrics** that are commonly used in the literature: the Very Simple Structure, empirical BIC, Velicer’s MAP, parallel analysis, the acceleration factor, and the optimal coordinate metric.
1. We prioritized a **data-driven approach**: empirical cross-validation where we applied EFA to half of the data and Confirmatory Factor Analysis (CFA) to the other half.
1. We also systematically decimated both the number of stimuli and the number of scales, testing for the stability of the results if the analysis was re-done on a randomly sampled subset of the data to ensure the **robustness** of our results.
1. We considered the **interpretability** of the final results based on factor loadings.

We then used EFA to extract three (‘valence’’, ‘‘arousal’’, and ‘‘generalizability’’), three (‘valence’’, ‘‘arousal’’, and ‘‘generalizability’’), and four (‘‘valence’’, ‘‘negative affect’’, ‘‘arousal’’, and ‘‘common’’) factors for the narrative-evoked, video-evoked, and real-life emotions, respectively.

To address possible concerns that our results may depend on the use of EFA, we further analyzed our data using **PCA, Autoencoders, and Principal Preserved Component Analysis (PPCA)**. All methods suggested a small number of dimensions to keep on the basis of cumulative proportion of variance explained and the nature of the first few dimensions was highly consistent across these different analytic methods.

In the aggregate, these different analyses provide the most convergent result that emotion experiences are characterized efficiently by **a low-dimensional space that includes valence and arousal**.

<h3 style="font-size: 1.0rem; text-decoration: underline; font-weight: bold; margin-bottom: 0.5rem;">
3.2 Distribution and Clustering:
</h3>

We next asked how different emotion experiences are distributed within this dimensional space and whether we could find evidence for clusters that might constitute discrete categories.

First, we projected data from the original high-dimensional spaces to two-dimensional spaces using **UMAP** for easier visualization and interpretation. Across all three types of emotion experiences, **valence emerged as a continuous global gradient, in line with the dimensional view of emotions**. Interactive versions of UMAP plots are available where each emotion experience can be inspected with the free responses collected in our study when users hover the mouse over the plots (<a href="/assets/html/emo_dim_narrative.html" style="font-weight:bold;">narrative</a>, <a href="/assets/html/emo_dim_video.html" style="font-weight:bold;">video</a>, <a href="/assets/html/emo_dim_reallife.html" style="font-weight:bold;">real-life</a>).

The qualitative observation of no discrete clustering structure from UMAP was supported by inspecting the distributions of pairwise Euclidean distances in the original high dimensional spaces. **We did not observe numerous peaks in the distributions that might have corresponded to discrete emotions**.

We tested whether the categories as defined semantically actually form clusters in the high dimensional space with clear boundaries in three different ways:

- **Hierarchical Clustering** revealed both within-category similarity and cross-category similarity.
- **K-means Clustering** solutions showed low agreement with the intended categories from the original studies.
- **A focused hierarchical clustering** on basic emotions failed to recover the intended categories even for these instances that were specifically chosen as the best examples of basic emotions.

The upshot from our data-driven approach is that we find **no evidence for discrete emotion clusters** and that instead emotion experience appears to be well described by a low-dimensional continuous space.

To summarize,

- Using a rich set of scales, we characterized the psychological space of emotion experiences evoked by a validated set of narratives, a validated set of videos, and actual experiences in real life during 2020.
- All three types of emotion experiences shared similar underlying low-dimensional structure, with the first two factors accounting for most of the variance corresponding to valence and arousal, in line with prior work.
- Our study discovered a dimension not previously reported, which we interpret as ‘‘generalizability’’: describing the degree to which an emotion is relatively modular and domain specific or domain general.
- Characterizing the distribution revealed that emotions were distributed along continuous gradients, with no well-separated clusters even for emotions belonging to the six basic emotion categories, contrary to theories postulating discrete emotion categories.

We acknowledge that, as with any study, our results are of course still limited by the choice we made on stimuli, tasks, and analytic methods. We provide a detailed discussion on how these choices shape the discovered dimensions of a psychological space in a separate review paper (published in _Affective Science_, {% cite lin2025review %}). I am also working on a paper on how individuals with alexithymia might differ in their emotion experiences evoked by our three stimulus types {% cite han&ralph2025_alexithymia %}.
