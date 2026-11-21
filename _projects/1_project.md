---
layout: page
title: "A Pedagogical Ray Tracer for Black Hole Imaging"
description: "An educational ray tracer for null geodesics and black hole images in Schwarzschild and Kerr spacetimes."
img: assets/img/research/PhotonRing.png
importance: 1
category: work
show_on_research: true
---

I developed a parallelized C++ ray-tracing code under the Schwarzschild and Kerr spacetime. These are the sample images obtained by my code.

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <img src="{{ '/assets/img/research/Sch_BH_disc_Iobs_movie.gif' | relative_url }}"
         alt="Ray-traced views of a Schwarzschild black hole and its surrounding disk"
         class="img-fluid rounded z-depth-1"
         loading="lazy">
  </div>
</div>
<div class="caption">
  Ray-traced views of a Schwarzschild black hole and its surrounding disk.
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <img src="{{ '/assets/img/research/BH_test_kerr_disc_Iobs_a10_movie.gif' | relative_url }}"
         alt="Ray-traced views of a Kerr black hole and its surrounding disk"
         class="img-fluid rounded z-depth-1"
         loading="lazy">
  </div>
</div>
<div class="caption">
  Ray-traced views of a Kerr black hole and its surrounding disk.
</div>

My earlier work used semi-analytical models informed by interpolation tables from smaller-scale simulations. That experience made me want to evolve the equations governing extreme phenomena near black holes more directly.

In undergraduate and graduate-level General Relativity courses at UT Austin, and Seoul National University, we derived geodesic equations and evaluated them for a given spacetime using its Christoffel symbols. But evolving these equations by hand is difficult, and I found that other students new to General Relativity often felt the same. I also heard that students wanted more intuitive observables, such as the black hole images in _Interstellar_. These needs, together with my previous research experience, led me to develop an educational ray tracer that lets students explore the equations and see the astrophysical images they produce.

I wrote the proposal independently and secured an approximately $2,000 research grant. Professor Sascha Trippe served as my faculty advisor and gave me generous, insightful guidance.

**Key Features**

- Integrates Hamiltonian equations for null geodesics in Schwarzschild and Kerr spacetimes.
- Produces relativistic images of black holes and their surrounding Keplerian disks, not just photon trajectories.
- Lets students vary the black hole spin, disk rotation direction, viewing inclination, and observer distance. With 8 CPU threads, it can generate 250 × 250 images in under 30 minutes.

**To Achieve This**

- I used the Hamiltonian formalism covered in my graduate-level General Relativity course at Seoul National University in Fall 2026.
- I modeled a geometrically thin, optically thick Keplerian disk extending from the ISCO to an adjustable outer radius, set to $20 R_g$.
- I used an observer-frame tetrad to convert intuitive photon directions into the coordinates used for each spacetime.
- I integrated rays backward in time with an RK4 integrator and tracked the Hamiltonian, angular momentum, and Carter constant to monitor numerical error.
- At each disk intersection, I enforced the null condition $H=0$, rather than estimating the hit by interpolating between neighboring integration steps.
- I wrote the code in C++ and used OpenMP for CPU parallelization.

The code is here! [repository](https://github.com/Hyun-kingofBH/TheLordofthePhotonRings).

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <img src="{{ '/assets/img/research/tshirt.jpg' | relative_url }}"
         alt="Hyun and friends wearing T-shirts printed with a ray-traced black hole image"
         class="img-fluid rounded z-depth-1"
         loading="lazy">
  </div>
</div>
<div class="caption">
  I printed a ray-traced image of a Schwarzschild black hole viewed at an inclination of 10° on T-shirts for a graduation photo with my wonderful friends at SNU in October 2026! Pictured with Jiseop Shin, I, Jong-In Park, and Yeongpyo Hong (left to right).
</div>
