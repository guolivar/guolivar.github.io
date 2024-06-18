---
layout: page
title: ODIN
description: Outdoor Dust Information Node
img: assets/img/odin_mountain_bg.jpg
importance: 5
category: work
nav: true
---

After our initial success with [PACMAN](../PACMAN), we decided to start working on an outdoor companion. At first, we used the same Sharp dust sensor that we put inside PACMAN but soon a new generation of laser-based optical particle sensors became available ([Plantower](https://aqicn.org/sensor/pms3003/)) and we upgraded our original ODIN that could only report an indicative measure of "dust", to being able to report $$PM_{10}$$, $$PM_{2.5}$$ and $$PM_1$$.
<div class="row justify-content-sm-center">
 <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/plantower3003.png" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

Initial tests showed that the Plantower sensors were much more consistent than the Sharp ones and that their response was much less affected by temperature. Also, tests in woodsmoke impacted areas showed an excellent performance of these devices.

<div class="row justify-content-sm-center">
 <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/odin_comparison_fdms.png" title="example image" class="img-fluid rounded z-depth-1" zoomable=true%}
  </div>
</div>

By 2018 we had upgraded our ODIN devices to use a 2G modem to send live data to our servers and being able to monitor in near-real time the air quality and were able to generate daily animations of the observed concentrations during the previous day. [You can see a sample animation here](https://vimeo.com/357097863)




[NIWA project page](https://niwa.co.nz/atmosphere/community-air-air-quality-issues-nz-towns/air-quality-monitoring-low-cost-sensors)