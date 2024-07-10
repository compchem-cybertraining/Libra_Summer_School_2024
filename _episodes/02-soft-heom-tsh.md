---
title: "2. Day 2: SOFT, HEOM, TSH and Ehrenfest with Model Hamiltonians"
---

# 1. Day info

 - July 9, 2024, Tuesday
 - Where: Clemens Hall 120
 - Instructors: Alexey Akimov

# 2. Model Hamiltonians 

## 2.1. Define model Hamiltonians (60 min)

[Slides](../files/Alexey_Akimov/July9-morning-Hamiltonian.pdf)

[Main directory](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/8_model_hamiltonians)

* Do the tutorial [1_pes_plotting](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/8_model_hamiltonians/1_pes_plotting)

* Explore the examples of [`some model Hamiltonians in Libra`](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/8_model_hamiltonians/3_models)

* Tasks: 

  - define your own 1-D or 2-D model Hamiltonian
 
  - plot the corresponding PESs and NACs


# 3. SOFT, TSH and Ehrenfest, and HEOM with Model Hamiltonians

## 3.1. SOFT calcultaions in Libra (60 min)

[Slides](../files/Alexey_Akimov/July9-morning-quantum.pdf)

Links:

[Main directory](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/6_dynamics/4_wavepackets)

* Do the tutorial [3_soft_propagation](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/6_dynamics/4_wavepackets/3_soft_propagation)

* Tasks:

  - explore several options of quantum dynamics propagation in the given tutorial (integrators, parameters, etc.)

  - run quantum dynamics for your Hamiltonian, keep it handy - we'll do TSH calculations with it later.


Links:

## 3.2. TSH and Ehrenfest dynamics with 1D model Hamiltonians (120 min)

[Slides, Part 1](../files/Alexey_Akimov/July9-afternoon-tsh-part1.pdf)

[Slides, Part 2](../files/Alexey_Akimov/July9-afternoon-tsh-part2.pdf)

[Slides, Part 3](../files/Alexey_Akimov/July9-afternoon-tsh-part3.pdf)

Links:

[Main directory](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/6_dynamics/1_trajectory_based)

* Complete the given tutorials:

  - [9_model_revised](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/6_dynamics/1_trajectory_based/9_model_revised)

  - [10_model_many_methods](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/6_dynamics/1_trajectory_based/10_model_many_methods)

  - [12_spin_boson_fmo](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/6_dynamics/1_trajectory_based/12_model_spin_boson_fmo)

* Tasks: 

  - run the TSH/Ehrenfest calculations for your potential using different methods:

        - try developing new recipes: hopping, rescaling, integrators, etc.

        - try different simulations: initial conditions, sampling, etc.

        - analyze the computed properties: energies, energy conservation, phase space portraits, etc.

        - compare to your results to the quantum results obtained in the morning

  - set up TSH/Ehrenfest calculations for a spin-boson Hamiltonian with 3 states and some 25 nuclear DOFs, save your results for later


## 3.3. HEOM for spin-boson Hamiltonian (60 min)

[Slides](../files/Alexey_Akimov/July9-afternoon-HEOM.pdf)

Links:

* Complete the given tutorial: [1_dynamics_and_lineshapes](https://github.com/compchem-cybertraining/Tutorials_Libra/tree/master/6_dynamics/3_heom/1_dynamics_and_lineshapes)

* Tasks: 

  - setup the HEOM calculations with the parameters related to your 3-state spin-boson model Hamiltonian 

  - compare the HEOM results with those of your TSH calculations obtained in the previous step



# 3. Videorecordings

## 3.1. UB Recording:

<iframe src="https://ub.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=010c5400-e29b-4eb7-9f75-b18f01178999
&autoplay=false&offerviewer=true&showtitle=true&showbrand=true&captions=false&interactivity=all" height="405" width="720" 
style="border: 1px solid #464646;" allowfullscreen allow="autoplay" aria-label="Panopto Embedded Video Player" 
aria-description="Libra Workshop and Summer School on Excited States and Nonadiabatic Dynamics 2024, Day 2" ></iframe>

## 3.2. Zoom recordings:

<iframe src="https://ub.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=a25ff470-a062-43f7-a03c-b1a80114c4d0
&autoplay=false&offerviewer=true&showtitle=true&showbrand=true&captions=false&interactivity=all" height="405" width="720" 
style="border: 1px solid #464646;" allowfullscreen allow="autoplay" aria-label="Panopto Embedded Video Player" 
aria-description="Libra Workshop and Summer School, Day 2, Part 1" ></iframe>


<iframe src="https://ub.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=1ac7db79-bf27-4ff0-8e39-b1a80162fb82
&autoplay=false&offerviewer=true&showtitle=true&showbrand=true&captions=false&interactivity=all" height="405" width="720" 
style="border: 1px solid #464646;" allowfullscreen allow="autoplay" aria-label="Panopto Embedded Video Player" 
aria-description="Libra Workshop and Summer School, Day 2, Part 2" ></iframe>


