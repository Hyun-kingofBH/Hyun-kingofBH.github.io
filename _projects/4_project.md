---
layout: page
title: "AGN Activity vs. SFR of the Host Galaxy: Type 1 AGN at 0.3 < z < 0.8"
description: "Studying the relationship between AGN activity and host galaxy star formation."
img:assets/img/AGN_feedback/coevo_thumbnail.jpg
importance: 4
category: work
---

From winter 2023 through winter 2024, I studied the relationship between AGN activity and the star formation rate (SFR) of host galaxies at Seoul National University. This was my first full research experience, and I am grateful to Professor Jong-Hak Woo for giving me this opportunity.

For galaxies with classical bulges and elliptical galaxies, studies have found correlations between SMBH mass and bulge properties, including bulge mass. Kormendy and Ho (2013) reviewed these relationships. They raise a broader question: how did SMBHs and their host galaxies grow together? I focused on the relationship between AGN activity and star formation in the host galaxies.

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid
       path="assets/img/AGN_feedback/coevo_thumbnail.jpg"
       title="Illustration of the coevolution of SMBHs and galaxies"
       class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  The chicken and egg question in astronomy: Which came first, AGN activity or galaxy growth?
  Figure from Marta Volonteri, “The Formation and Evolution of Massive Black Holes,”
  <em>Science</em>, 337, 544–547 (2012).
  <a href="https://doi.org/10.1126/science.1220843" target="_blank" rel="noopener">
    DOI: 10.1126/science.1220843
  </a>
</div>

**AGN sample and activity indicators**

I studied about 5,500 Type 1 AGNs at $0.3<z<0.8$ from the SDSS quasar catalog. I used the 5100 Å continuum luminosity and the effective outflow velocity measured from the [O III] &lambda;5007 line in the SDSS spectra as proxies for AGN activity.

**Estimating host galaxy SFR**

Because AGN emission can contaminate the H$\alpha$ line in Type 1 AGNs, estimating host galaxy SFR from spectroscopy alone is challenging. I used CIGALE to fit the targets’ multiwavelength photometry, from UV to FIR, including data from GALEX, 2MASS, WISE, and IRAS.

Only 136 of the approximately 5,500 AGNs had FIR data. I compared the SFR estimates with and without FIR photometry for those objects. The estimates were broadly consistent, with an RMS difference of 0.32 dex. This comparison allowed me to estimate SFRs for the rest of the sample, which lacked FIR data.

In this sample, I found no strong evidence that AGN activity immediately suppresses star formation in the host galaxies.

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid
       path="assets/img/AGN_feedback/CIGALE.jpg"
       title="CIGALE SED fits with and without FIR photometry"
       class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  CIGALE SED fits without FIR photometry (left) and with FIR photometry (right).
  I compared the SFR estimates for every object with FIR data and found them broadly
  consistent, with an RMS difference of 0.32 dex. This allowed me to estimate SFRs
  for the other AGNs without FIR data.
</div>

<!-- Add the poster section after permission to share the poster PDF.

This is the poster I presented at the Korean Astronomical Society meeting in 2024.

<a href="{{ '/assets/img/AGN_feedback/POSTER_FILE.pdf' | relative_url }}"
   target="_blank"
   rel="noopener">
  Open the poster PDF
</a>

-->
