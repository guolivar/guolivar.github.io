---
layout: page
title: PACMAN
description: Particles, Activity and Context Monitoring Autonomous Node
img: assets/img/pacman.jpg
importance: 6
category: work
nav: true
---
Back in 2012, NIWA was conducting a wood-burning emission measurement campaign in Christchurch (New Zealand) and just because we had one not being used, we installed a SidePak in the participant's livingroom and then we found that the concentrations indoors were most of the time much larger than outdoors and with peaks that were not always corresponding to when the woodburner was being re-loaded:
<div class="row justify-content-sm-center">
  <div class="col-sm-3 mt-3 mt-md-0">

    {% include figure.liquid path="assets/img/chch_indoor_out.png" title="Indoor and Outdoor PM10" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
  <div class="col-sm-3 mt-3 mt-md-0">

    {% include figure.liquid path="assets/img/indoor_peaks.png" title="Indoor PM10" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>

So, we needed an instrument to observe what was happening at the time of these high concentration events. Our basic requirements were:

*  Small form factor
* Non-intrusive
* Low cost
* Air Quality characterisation:
    * Particulate matter 
* Context and activity characterisation
    * Presence
    * Temperature
    * Activity 

And that's how PACMAN (Particles, Activity and Context Measurement Autonomous Node) was born (yes, the acronym is a little contrived but ... PACMAN!!). The whole design process was open source (GPL3 license) and more detailed information can be found [in the Bitbucket repository](https://bitbucket.org/guolivar/pacman) along with all the design files.

Here is a sample of one day of measurements in a home to show that the device was capable of capturing a number of features related to the context of the indoor air quality measurements.
{% include figure.liquid path="assets/img/pacman_test_data1.png" title="PACMAN data" class="img-fluid rounded z-depth-1" zoomable=true %}






