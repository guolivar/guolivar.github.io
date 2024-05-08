---
layout: page
title: Clear the air
description: improving ventilation practices in NZ
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

When it became clear that New Zealand's successful [elimination strategy](https://www.theguardian.com/world/commentisfree/2022/apr/05/new-zealands-covid-strategy-was-one-of-the-worlds-most-successful-what-can-it-learn-from-it) was to be replaced with one of [mitigation](https://www.reuters.com/world/asia-pacific/new-zealand-extends-auckland-lockdown-eases-some-curbs-2021-10-04/), it became clear that we needed to understand the ventilation practices in our indoor spaces.

As part of the Ministry of Health fund to improve preparedness for future pandemics, my team set out to characterise the ventilation conditions of multiple indoor spaces in New Zealand. In order to do that, we had to develop a system that would be able to measure $$CO_2$$ as well as context information such as human presence, and open/close state of doors and windows.

Our response to this challenge was to develop SHAQS (Smart Home Air Quality System), a modular and portable system to quickly characterise the ventilation performance of indoor spaces. The heart and brain of the system is a Raspberry Pi computer running [Home Assistant](https://www.home-assistant.io/) that receives the data transmissions form air quality sensors as well as human presence monitors and door/window opening sensors.
The parameters measured are:
* Motion detection. mmWave radar (Tuya ZigBee Human Presence Detector)
* Door/Windows opening sensor. Simple Hall sensors with ZigBee connectivity (Tuya ZigBee Door Window sensor)
* Indoor air quality. The Qingping Air Monitor Lite using BlueTooth connectivity:
  + CO2. Photoacoustic sensor – Sensair 41.
  + PM1, PM2.5, PM10. Plantower PMS5003 laser dust sensor.

[NIWA project page](https://niwa.co.nz/atmosphere/reducing-covid-19-transmission-through-increased-ventilation)

<!--
Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>

</div>
<div class="caption">

    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.

</div>
<div class="row">

    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>

</div>
<div class="caption">

    This image can also have a caption. It's like magic.

</div>

You can also put regular text between your rows of images, even citations {% cite einstein1950meaning %}.
Say you wanted to write a bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, _bled_ for your project, and then... you reveal its glory in the next row of images.

<div class="row justify-content-sm-center">

    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>

</div>
<div class="caption">

    You can also have artistically styled 2/3 + 1/3 images, like these.

</div>

The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```

{% endraw %}
-->
