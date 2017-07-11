# Goal and Plan Recognition Dataset
[![DOI](https://zenodo.org/badge/76881547.svg)](https://zenodo.org/badge/latestdoi/76881547)

This repository contains datasets for goal and plan recognition as planning.

We created these datasets to evaluate goal/plan recognition approaches that use planning techniques.

We added 15 datasets with missing and full observations, and 4 datasets with missing and noisy observations.

- Six of these datasets were created by Ramírez and Geffner, and they are available in: https://sites.google.com/site/prasplanning/. Based on these six datasets, which contain hundreds of goal/plan recognition problems, we added larger planning problems and generated new datasets from the remaining 9 planning domains;
- The datasets with missing and noisy observations were generated based on the code provided by Sohrabi in https://github.com/shirin888/planrecogasplanning-ijcai16-benchmarks;

Each .tar.bz2 file represents a goal/plan recognition problem, containing a domain description (domain.pddl), an initial state (template.pddl), a set of candidate goals (hyps.dat), a correct hidden goal in the set of candidate goals (real_hyp.dat), and an observation sequence (obs.dat). 
An observation sequence contains actions that represent an optimal plan or sub-optimal plan that achieves a correct hidden goal, and this observation sequence can be full or partial. 
A full observation sequence represents the whole plan for a hidden goal, i.e., 100\% of the actions having been observed. 
A partial observation sequence contains missing observations and represents a plan for a correct hidden goal with 10\%, 30\%, 50\%, or 70\% of its actions having been observed. For goal/plan recognition problems with noisy observations, the observability of partial observations is quite different because every observation sequence always includes 2 noisy observations, so a partial observation sequence with noisy observations represents a plan with 25\%, 50\%, or 75\% of its actions having been observed.

These datasets were used in the experiments described in [Landmark-Based Heuristics for Goal Recognition](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14666).
