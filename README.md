# Random Walk Metropolis–Hastings: MCMC Sampling & Convergence Diagnostics

A **from-scratch implementation** of the **Random Walk Metropolis (RWM)** algorithm—a **Markov Chain Monte Carlo (MCMC)** method—for sampling from a **Laplace distribution** and assessing convergence using the **Gelman–Rubin (\(R_b\)) diagnostic**.

> **Language:** Python  
> **Libraries:** NumPy, Matplotlib, Seaborn

---

## Overview

Many probability distributions cannot be sampled from directly using standard techniques. Markov Chain Monte Carlo (MCMC) methods overcome this by constructing a Markov chain whose long-run behaviour converges to the desired target distribution.

This project implements the **Random Walk Metropolis algorithm** from scratch to generate samples from the Laplace distribution

\[
f(x)=\frac{1}{2}e^{-|x|}
\]

and evaluates the quality of the sampler using Monte Carlo estimation and convergence diagnostics.

---

## Project Objectives

This project:

- Implements the **Random Walk Metropolis (RWM)** algorithm from scratch.
- Generates samples from a **Laplace distribution** without direct sampling.
- Validates the sampler using histograms, kernel density estimation (KDE), and Monte Carlo estimates.
- Assesses convergence using multiple independent Markov chains and the **Gelman–Rubin (\(R_b\)) diagnostic**.
- Investigates how the proposal step size affects convergence and mixing behaviour.
