---
layout: page
title: Clear the air
description: Improving ventilation practices in NZ
img: assets/img/clearair01.jpg
importance: 1
category: work
related_publications: false
nav: true
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

The data are streamed to an InfluxDB instance with a separate bucket for each SHAQS. Data available locally onboard of each SHAQS only covers the last 48 hours. To generate the automatic reports, we setup Batch jobs in Amazon's cloud computing platform to run Docker images with R scripts to take the data from the InfluxDB database and generate automatic daily and weekly reports.

[NIWA project page](https://niwa.co.nz/atmosphere/reducing-covid-19-transmission-through-increased-ventilation)
