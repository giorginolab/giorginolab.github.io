---
layout: post
date: 2026-11-20
title: cuPotential benchmarks on Leonardo
inline: false
summary: On a single A100 GPU, NVIDIA’s cuPotential ran DHFR simulations 2.6–3.1× as fast as standard OpenMM with CHARMM36 and CHARMM36m after we reorganized the Lennard-Jones terms.
---

I’ve shared scripts for running NVIDIA’s cuPotential with OpenMM on the Leonardo supercomputer. In addition to AMBER, we benchmarked CHARMM36 and CHARMM36m for DHFR on a single A100 GPU. In OpenMM’s default CHARMM36 setup, cuPotential speeds up electrostatics, but the separate Lennard-Jones calculation limits the overall gain to 2–11%. We (meaning me + Claude) moved the Lennard-Jones terms that follow standard mixing rules into the force that cuPotential accelerates and kept CHARMM36m’s pair-specific corrections in OpenMM. With this change, cuPotential ran 2.6–3.1× as fast as standard OpenMM using the same reorganized force terms. [Setup instructions, benchmark results, and run logs](https://github.com/giorginolab/cuPotential-leonardo)
