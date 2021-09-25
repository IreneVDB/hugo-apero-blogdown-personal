---
title: "Onze Lucht"
subtitle: "An R Shiny app for air quality sensors in the Netherlands"
excerpt: "Onze Lucht is a citizen science project in the North of the Netherlands where citizens use home-build sensors to measure air quality (PM2.5, PM10), temperature and humidity. I created an R Shiny app that visualizes monthly air quality in interactive heatmaps."
date: 2021-07-01
author: "Irene van den Broek"
draft: false
tags:
  - RShiny
categories:
  - RShiny
  - R
  - Environment
layout: single
links:
- icon: link
  icon_pack: fas
  name: Website
  url: https://onzelucht.nl
- icon: r-project
  icon_pack: fab
  name: Shiny App
  url: https://jebentwatjemeet.shinyapps.io/OnzeLucht/
- icon: github
  icon_pack: fab
  name: Code
  url: https://github.com/IreneVDB/OnzeLucht
---

## Onze Lucht

![Onze Lucht Logo](OnzeLucht.png)

[Onze Lucht](https://onzelucht.nl) is a citizen science project where citizens in the North of the Netherlands monitor air quality in their living environment using home-build sensors that measure PM2.5, PM10, temperature and humidity. <p>
I created an **R Shiny** app that allows participants to access their monthly data using their personal sensor-id. The monthly data is visualized in **interactive heatmaps** created with `ggplotly` based on the static heatmaps illustrated below.

You can view the R Shiny app on [shinyapps.io](https://jebentwatjemeet.shinyapps.io/OnzeLucht/)

---

### Air Quality PM2.5

![Heatmap with Air Quality PM2.5 Data](P25.png)

---

### Air Quality PM10

![Heatmap with Air Quality PM10 Data](P10.png)

---

### Temperature

![Heatmap with Temperature Data](Temperature.png)

---

### Humidity

![Heatmap with Temperature Data](Humidity.png)
