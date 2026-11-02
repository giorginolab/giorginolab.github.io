---
layout: page
title: Software
nav_title: Software
permalink: /software/
nav: true
nav_order: 4
---

I've authored or contributed to a number of open-source software packages in the field of computational statistics and physics.

- The [SCov2-MD](http://www.scov2-md.org/) database
  - Allowing the evolution-structure-dynamics-phenotype multidimensional analysis on SARS-CoV-2 genomes. Described in the paper [SCoV2-MD: a database for the dynamics of the SARS-CoV-2 proteome and variant impact predictions](https://doi.org/10.1093/nar/gkab977), published in Nucleic Acid Research as a Breakthrough article.
- The [Dynamic Time Warping project](https://dynamictimewarping.github.io/)
  - Providing packages and information on an extensive array of [DTW-style algorithms in both R and Python](https://dynamictimewarping.github.io/). The DTW algorithm computes the time axis stretch which optimally maps one timeseries (query) onto another (reference). The packages provide the most complete, freely-available (GPL) implementation of Dynamic Time Warping-type (DTW) algorithms up to date. They are described in the (~1000 citations) paper [Computing and Visualizing Dynamic Time Warping Alignments in R: the dtw Package.](http://www.jstatsoft.org/v31/i07)
- The [MYSEC-PM (Secondary Myelofibrosys Prognostic Model) model](http://www.mysec-pm.eu/).
  - A model and the corresponding online calculator described in A clinical-molecular prognostic model to predict survival in patients with post polycythemia vera and post essential thrombocythemia myelofibrosis. Leukemia 31, 2726–2731 (2017) [doi:10.1038/leu.2017.169](http://dx.doi.org/10.1038/leu.2017.169) . The MYSEC-PM model is now adopted in the NCCN Clinical Practice Guidelines in Oncology guidelines.
- The [PYCV module for PLUMED 2](https://giorginolab.github.io/plumed2-pycv/)
  - Enables [PLUMED2](https://www.plumed.org/) Collective Variables (CVs) and arbitrary functions to be defined and auto-differentiated in the Python language. Described in the paper [PYCV: a PLUMED 2 Module Enabling the Rapid Prototyping of Collective Variables in Python](https://doi.org/10.21105/joss.01773)
- Protein preparation for in silico experiments.
  - The preparation includes titration of the protonation states using PROPKA 3.1 and overall optimization of the H-network using PDB2PQR 2.1. Available online, as part of [Playmolecule's ProteinPrepare](https://www.playmolecule.org/proteinPrepare/), and in [HTMD](https://www.htmd.org//) (High Throughput Molecular Dynamics), See also the [introductory talk](https://secure.acellera.com/htmd-workshop-2016/03_PreparationBuilding_TGiorgino.tgz) at the 3rd HTMD workshop. doi:[10.1021/acs.jcim.7b00190](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.7b00190)
- The [ECL2 database](http://ecl2.giorginolab.it/).
  - The extracellular loop 2 (ECL2) is the longest and the most diverse loop among class A G protein-coupled receptors (GPCRs). We proposed a 7-cluster classification scheme of currently resolved ECL2 domains based on volume overlaps and their intermolecular interactions with the other GPCR regions.
- [METAGUI version 3](https://github.com/metagui/metagui3).
  - METAGUI extends VMD with a graphical user interface that allows constructing a thermodynamic and kinetic model of a given process simulated by long-scale molecular dynamics. It is described in [doi:10.1016/j.cpc.2017.04.009](https://doi.org/10.1016/j.cpc.2017.04.009)
- The PLUMED2 Metric in [HTMD](https://www.htmd.org//)
  - The MetricPlumed2 class allows the use of arbitrary PLUMED2 collective variables in the construction of Markov models within HTMD. See the [introductory talk](https://secure.acellera.com/htmd-workshop-2016/99_MetricPlumed2_TGiorgino.tgz) at the 3rd HTMD workshop.
- A web service, [infix2pharmml](http://infix2pharmml.sourceforge.net/) for the pharmacometrics language [PharmML](http://www.pharmml.org/).
  - The software converts the conventional mathematical infix notation into the math markup used by the pharmacometrics language [PharmML](http://www.pharmml.org/); the rationale is explained in [doi: 10.1002/psp4.57](http://onlinelibrary.wiley.com/doi/10.1002/psp4.57/abstract)
- The [MEMBPLUGIN](https://sourceforge.net/projects/membplugin/) membrane plugin analysis suite for VMD.
  - MEMBPLUGIN is a membrane analysis tool for molecular-dynamics simulations. It is a collection of visual and command-line tools that can be run within the Visual Molecular Dynamics (VMD) environment to analyze biomolecular simulations of lipid bilayers. It is described in the paper [MEMBPLUGIN: studying membrane complexity in VMD.](http://dx.doi.org/10.1093/bioinformatics/btu037)
- The [Plumed-GUI collective variable analysis tool](https://github.com/tonigi/vmd_plumed)
  - VMD plugin provides convenient access to the extensive set of collective variables (CV) defined in the PLUMED software. It allows the use of PLUMED syntax to conduct analysis on MD trajectories, and a convenient interface to prepare the metadynamics CV definitions. It is described in the paper [Plumed-GUI: an environment for the interactive development of molecular dynamics analysis and biasing scripts.](http://dx.doi.org/10.1016/j.cpc.2013.11.019)
- The [VMD Density Profile Tool](https://github.com/tonigi/vmd_density_profile)
  - The Density Profile Tool is a VMD analysis plugin that computes 1-D projections of various atomic densities. It's described in the paper [Computing 1-D atomic densities in macromolecular simulations: The density profile tool for VMD.](http://www.sciencedirect.com/science/article/pii/S0010465513002956)
- The [Diffusion Coefficient Tool](https://github.com/tonigi/vmd_diffusion_coefficient)
  - An analysis plugin for VMD that computes one, two or three-dimensional diffusion coefficients during a loaded trajectory based on average mean square displacements. Described in [Computing diffusion coefficients in macromolecular simulations: the Diffusion Coefficient Tool for VMD](https://joss.theoj.org/papers/10.21105/joss.01698)
- The [RBoinc system](http://boinc.berkeley.edu/trac/wiki/RemoteJob) (distributed computing as a virtual supercomputer)
  - RBoinc extends the Berkeley Open Infrastructure for Network Computing (BOINC), the open-source middleware for distributed computing projects, with mechanisms to submit and manage large-scale distributed computations from individual workstations. It is described in the paper [Tools to run and manage large-scale BOINC simulations](http://boinc.berkeley.edu/rboinc.pdf)(2010).
- [VMD extension functions](http://tonigi.github.io/vmd_extensions/)
  - a collection of TCL-VMD functions and iterators that support extraction of structural data from large-scale simulations. They provide simple semantics to iterate a block of code over frames or trajectory files, functions to compute the number of native contacts, distance matrices, and more.
- [Upper-limb rehabilitation exercises acquired through 29 elastomer strain sensors placed on fabric](http://dx.doi.org/10.5281/zenodo.11229).
  - A multivariate dataset obtained recording the stretch of various segments of the fabric of a sensorized garment while executing several rehabilitation exercises. Open data at [Zenodo](http://dx.doi.org/10.5281/zenodo.11229).

### Past projects

- Earlier research focused on the modelling of biomolecular recognition in [unstructured proteins](http://en.wikipedia.org/wiki/Intrinsically_unstructured_proteins), a wide class of proteins, whose detailed mechanisms of action are largely undetermined, and on [multi-scale simulation and prediction of the drug safety problems related with hERG](http://www.vph-noe.eu/exemplarprojects?start=4) within the Virtual Physiological Human Network of Excellence.
- [MyHeart's NeuroRehab](http://www.labmedinfo.org/projects/myheart) project (2005-2008) The NR platform supports physicians and therapists in the delivery of personalized exercise plans. The recovery process supports both motor rehabilitation exercises, which are monitored with kinestetic strain-sensor garments, and cognitive rehabilitation. The project involved the creation of the mathematical models, refinement of algorithms, and development of hardware and software, up to the clinical tests of the prototypes. (See [video](http://vimeo.com/896814) and [publications]({{ '/publications/' | relative_url }}))
- [AdaRTE dialog management](http://www.labmedinfo.org/projects/adarte) system for the medical domain (lead, 2002-2008) The proposal set forth in my PhD thesis (AdaRTE, a framework to support automated spoken dialogues in telemedicine) was developed into a system which is now used routinely in teaching, research, and to realize dialog systems used in the clinic. (See [publications]({{ '/publications/' | relative_url }}))
- Formerly, I worked with the APE collaboration in Pisa and DESY-Zeuthen (Berlin), profiling the hardware and compilation chain of the ApeNEXT massively-parallel dedicated super computer during its development.
  - Performance evaluation of the ApeNEXT processor during development: [ApeNEXT: Architettura ed algoritmi di LGT](http://www-zeuthen.desy.de/apewww/APE/publications/toniGiorgino_thesis.pdf) (2001)
  - Preliminary GCC target for the ApeNEXT floating-point architecture (2001)
  - Kernel drivers: zero-copy [AMCC S6855 kernel driver](https://github.com/acisternino/amcc-s5933-linux-drivers) (1999)
  - The linux kernel: [CDROM_SELECT_SPEED ioctl](https://lxr.linux.no/linux-old+*/drivers/ide/ide-cd.c#L191) (1998)

### Superseded software

- [RMSD trajectory tool enhanced with native contacts](https://github.com/tonigi/vmd_rmsdttnc)
  - enables VMD to compute the number of native contacts in a trajectory. It is an extension of the RMSD Trajectory Tool, of which it shares the interface.
- The [PdbTer](http://www.multiscalelab.org/utilities/PdbTer) plugin
  - allows VMD to write PDB files with TER cards separating molecules, as required by the PDB standard and some molecular-manipulation software (notably, tleap and xleap).
- Full "Save as" for VMD
  - A [function](http://tonigi.github.io/vmd_extensions/group__save.html) to (almost) save the complete state of a VMD session. Saved state includes the view, materials, colors (as with the usual save state menu item), as well as trajectories and topologies. This way, you can save and resume working on an image. Now part of the [VMD extension functions](http://tonigi.github.io/vmd_extensions/).
- The [Cast structure tool](http://www.multiscalelab.org/utilities/CastStructureTool), a modeling plugin which copies the coordinates of a selection A from another selection B, preserving A's topology. Coordinates of A's atoms will be copied verbatim when an unambiguous match exists in B; otherwise, the new coordinates will be guessed with a local fit.
