# Computational Biology Project: Design and Implement simple individual-based simulations of evolution
Simulation of evolutionary dynamics in asexual populations using individual-based models and Fisher’s Geometrical Model (FGM).
The project explores how mutation rates, environmental changes, and phenotypic complexity influence evolutionary adaptation.


# Project Overview

This project implements an individual-based simulation of evolutionary dynamics in microbial populations.
The model combines:
- Fisher’s Geometrical Model (FGM) to represent phenotype–fitness relationships
- A non-neutral Moran process to simulate reproduction and selection
- A mutator allele controlling mutation rate

The goal is to study how mutation rate evolution affects adaptation and population dynamics.
The simulations reproduce classical evolutionary phenomena observed in microbial populations.

# Key Research Questions

The project investigates:
- When mutator alleles can spread in a population
- How mutation rate affects adaptation speed and efficiency
- Whether punctuated equilibrium can emerge from simple evolutionary dynamics
- The effect of phenotypic complexity on adaptation
- How populations respond to changing environments

# Model Description

Each individual is represented as a point in a d-dimensional phenotypic space.
Fitness depends on the distance from an environmental optimum, modeled with a Gaussian fitness landscape according to Fisher’s Geometrical Model.
Evolution proceeds through a Moran birth–death process:
-One individual reproduces with probability proportional to fitness
-One individual is randomly removed
-The offspring inherits phenotype and mutator status, possibly with mutation
-Mutations modify a subset of phenotypic traits and can be beneficial or deleterious depending on their effect on fitness.

# Experiments
The simulation explores several evolutionary scenarios:

1) Mutator allele competition
Study of fixation probability of mutator alleles depending on initial frequency.

2) Mutation rate strength
Analysis of how increasing mutation rate affects adaptation speed and long-term fitness.

3) Punctuated equilibrium
Simulations show long periods of evolutionary stasis interrupted by sudden adaptive jumps.

4) Phenotypic complexity
Increasing the number of phenotypic traits reduces the availability of beneficial mutations and slows adaptation.

5) Moving environmental optimum
Simulations of changing environments reveal different regimes:
-extinction under rapid environmental change
-near-perfect adaptation for slow changes
-Red Queen dynamics at intermediate speeds.

# Technologies
Python (NumPy, Matplotlib)
