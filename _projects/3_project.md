---
layout: page
title: "How Far Can JWST Observe SMBHs?"
description: "Estimating how far JWST can detect and identify growing SMBHs."
img: assets/img/SMBH_JWST/SMBH_thumbnail.png
importance: 3
category: work
show_on_research: true
---

I investigated how far JWST could detect and tentatively identify SMBHs through photometry and spectroscopy. I began this project by asking whether JWST could eventually distinguish light seed and heavy seed models, helping us understand how SMBHs formed. I was fortunate to work with Professor Volker Bromm during my exchange semester at UT Austin in 2025, and I remain grateful for his warm support and academic inspiration. I am also thankful for my wonderful collaborators.

Observations of quasars with masses above $10^7\,M_\odot$ at $z>6$ raise a puzzle: how could black holes that began as small stellar mass seeds grow so rapidly within the first billion years of the Universe? To address this puzzle, alternative heavy seed scenarios have been actively studied including direct collapse black holes. Although these models alleviate the black hole timing mystery, their growth and interaction with their surroundings may erase clues to a black hole’s initial seed, making it difficult to probe directly. Estimating JWST’s detection limits can help guide strategies for upcoming surveys.

**Photometric detectability**

I traced SMBH growth under different seed and accretion histories. I then applied a fiducial photometric sensitivity threshold to estimate the redshift horizon in three scenarios:

- Feedback regulated growth
- Light seed growth with continuous super Eddington accretion
- Direct collapse black holes, or heavy seeds, with continuous Eddington accretion

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid
       path="assets/img/SMBH_JWST/LS_sup_timeax.png"
       title="Example of SMBH growth from a light seed"
       class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Example of SMBH growth from a light seed. In this optimistic scenario, continuous super Eddington accretion allows the SMBH to reach $10^7\,M_\odot$ at a higher redshift.
</div>

**Spectroscopic identification**

Photometric detectability alone cannot confirm an AGN, so I also examined whether spectral features could provide an AGN signature. At $z>10$, H$\alpha$ and H$\beta$ shift beyond NIRSpec’s wavelength range. MIRI reaches longer wavelengths, but its sensitivity limits these lines for sources in the scenarios we modeled. I therefore examined high ionization lines such as $\mathrm{N\,V}\,\lambda1240$ as potential indirect AGN signatures.

Under our optimistic growth scenarios and adopted sensitivity assumptions, our estimates suggest that JWST may detect and identify SMBHs out to $z\sim16$, potentially probing them closer to their origin. Our paper is submitted to the Astrophysical Journal in November 2026!

<div class="caption">
  Thumbnail image: Illustration by NASA, ESA, CSA, and Ralf Crawford (STScI). See the
  <a href="https://science.nasa.gov/asset/webb/flaring-disk-around-milky-ways-black-hole-artists-concept/"
     target="_blank"
     rel="noopener">NASA image page</a>.
</div>
