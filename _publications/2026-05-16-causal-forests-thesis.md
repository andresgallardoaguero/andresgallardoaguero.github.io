---
title: "Do Causal Forest Methods Identify the Right Sources of Treatment Effect Heterogeneity? Evidence from Clinical Data with Known Ground Truth"
collection: publications
category: research_in_progress
permalink: /publication/causal-forests-thesis
date: 2026-05-16
venue: "Master's thesis, University of St. Gallen (in progress)"
excerpt: "Master's thesis at the University of St. Gallen, supervised by Prof. Dr. Jana Mareckova and Dr. Justus Vogel. A simulation study with known ground truth that evaluates whether causal forest methods and their variable importance measures correctly identify the variables driving heterogeneous treatment effects in clinical data."
---

Master's thesis at the University of St. Gallen, supervised by Prof. Dr. Jana Mareckova and co-supervised by Dr. Justus Vogel. Expected submission: 17 November 2026.

The thesis is a simulation study with known ground truth that asks two questions about causal forest methods. First, whether the variable importance measures of these methods correctly identify the variables that drive heterogeneous treatment effects. Second, how reliably the underlying estimators (Generalized Random Forests and Modified Causal Forests) recover those effects to begin with.

The simulation calibrates its covariate marginals, correlation structure, and treatment prevalence to ICU patient data from the surgical ICU cohort at the Cantonal Hospital of St. Gallen, while imposing synthetic potential outcomes on top so the true CATE function is known by construction. The design varies five structural features of the data-generating process (confounding strength, heterogeneity strength, modifier sparsity, proxy correlation, and CATE distribution shape) across a 32-cell factorial grid.

Five variable importance methods spanning four methodological categories are compared on the same construction-known truth: GRF split-frequency, MCF OOB-permutation, the Hines TE-VIM (LOCO-based, model-agnostic), the Bénard and Josse drop-and-relearn measure (forest-specific), and PermuCATE (conditional-permutation-based, model-agnostic). Evaluation uses precision-recall against the binary truth set of variables in the CATE function, rank correlation against the Hines variance functional, and type I error and power for the methods that admit formal hypothesis tests. A welfare-regret layer translates methodological disagreements into patient-outcome units under a stylized treatment-assignment rule.
