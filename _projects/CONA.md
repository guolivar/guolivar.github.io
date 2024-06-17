---
layout: page
title: CONA
description: Community Observation Networks for Air
img: assets/img/odin_mountain_bg.jpg
importance: 4
category: work
nav: true
---

Starting in 2015 with the first versions of our ODIN (Outdoor Dust Information Node) we set out to change the way air quality is managed in New Zealand by empowering the communities to engage with the local authorities to identify their most important air quality problems and to co-develop solutions that will reduce their exposure to air pollution.

Therefore, the central theme of the CONA projects was the use of low-cost, distributed sensor networks focusing on woodsmoke and on enabling local communities to participate in the evaluation of the measurements.

My role in these projects was first to develop and maintain the hardware used ([ODIN](../ODIN) first and then [Clarity](https://clarity.io) devices) as then to implement a suitable data infrastructure that would allow us to take the raw measurements and turn them into information that the community and the environmental managers could use to inform their discussions.

While ODIN is described in more detail [here](../ODIN), the data infrastructure developed for these projects was:

* PostgreSQL database to centralise the data flow from the devices data backends.
* R and Python scripts to move data from the telemetry backend to the long-term storage PostgreSQL database.
* Docker images to run diagnostics and reporting scripts on demand and on schedule to generate:
    * Daily data capture diagnostics for all devices
    * Daily spatial averages for all the deployments
    * Daily files for 3D visualisation of the previous day's air quality




[NIWA project page](https://niwa.co.nz/atmosphere/community-observation-networks-air-cona-previous-projects)