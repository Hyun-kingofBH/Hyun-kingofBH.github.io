---
layout: page
title: "Multiple Massive Black Hole Systems in the LUMINA"
description: "Modeling high-redshift MBH binaries, potential dual AGN, and triplets in the LUMINA cosmological simulation."
# All images and PDFs of this project live in ONE folder: assets/img/projects/2_project/
# (same name as this file). To add a file, put it in that folder and refer to it as
# assets/img/projects/2_project/FILE_NAME. "img" below is the card thumbnail on /research/.
img: assets/img/projects/2_project/LUMINA_thumbnail.png
importance: 2
category: work
show_on_research: true
---

Since February 2026, I have been studying the populations of potential dual AGN and massive black hole (MBH) pairs detectable by LISA at high redshift ($3 \gtrsim z \lesssim 7$). Using LUMINA’s large volume, I also extended the analysis beyond binaries to study higher-order systems including MBH triplets. I work with Dr. Oliver Zier, PI of the LUMINA simulation, and Dr. Jacob Shen at the Harvard Center for Astrophysics.

Galaxy mergers are common over a galaxy's lifetime, and most massive galaxies are thought to host an MBH at their center. What happens to these central MBHs when their host galaxies merge? Do they eventually merge to form a larger MBH, or can they persist as a binary for a long time? These questions have long interested me.

<div class="row">
  <div class="col-md-6 mt-3 mt-md-0">
    <img src="{{ '/assets/img/projects/2_project/Bigblackhole.png' | relative_url }}"
         alt="Illustration of a massive black hole"
         class="img-fluid rounded z-depth-1"
         loading="lazy">
    <div class="caption">
      Will they merge into a larger SMBH?
    </div>
  </div>

  <div class="col-md-6 mt-3 mt-md-0">
    <img src="{{ '/assets/img/projects/2_project/MBHB.png' | relative_url }}"
         alt="Illustration of a massive black hole binary"
         class="img-fluid rounded z-depth-1"
         loading="lazy">
    <div class="caption">
      Or will they persist as binaries for a long time?
    </div>
  </div>
</div>

**How do we study multiple MBH systems?**

- I analyze black hole merger trees to estimate the abundance of MBH binaries.
- I use Holodeck, a subgrid modeling software, to model unresolved MBH binary inspirals. It includes dynamical friction, stellar loss-cone scattering, viscous hardening by circumbinary disks, and gravitational-wave emission.
- I connect LUMINA to Holodeck by extracting host-galaxy properties for black holes that have merged in LUMINA and using them as initial conditions for Holodeck.
- I evolve the binaries with Holodeck to estimate their abundance at different redshifts.
- I use a fiducial rest-frame UV luminosity as an observability criterion to estimate an optimistic population of potential dual AGN.

**What have we found?**

The poster below presents preliminary results that I shared at the 2026 Summer School of NR and GW in Daejeon, Korea. Some model parameters and the definition of an MBH triplet differ from our current analysis. We aim to submit the paper by January 2027 and will share the final results after submission.

<p>
  <a href="{{ '/assets/img/projects/2_project/Hyun_NRGW2026.pdf' | relative_url }}"
     target="_blank"
     rel="noopener">
    Open the poster PDF in a new tab
  </a>
</p>

<iframe src="{{ '/assets/img/projects/2_project/Hyun_NRGW2026.pdf' | relative_url }}"
        title="Preliminary LUMINA research poster"
        style="width: 100%; height: 850px; border: 0;">
</iframe>
