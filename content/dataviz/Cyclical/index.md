---
title: "Circles and Cycles"
subtitle: "Female cycle"
excerpt: "Cyclical timeseries"
date: 2019-07-01
author: "Irene van den Broek"
draft: true
image:
  caption: ''
  focal_point: Smart
tags:
categories:
layout: single
links:
- icon: link
  icon_pack: fas
  name: docs?
  url: https://onzelucht.nl
- icon: github
  icon_pack: fab
  name: Code
  url: https://github.com/IreneVDB/OnzeLucht
---

Cirkelvormige datavisualisaties
Cirkelvormige datavisualisaties, denk bijvoorbeeld aan het taartdiagram, de donut plot, cirkelvormige staafdiagrammen, het Venn diagram of zogenaamde spinnenweb- of radarplots, ogen vaak erg mooi. Maar het belangrijkste van een goede datavisualisatie is natuurlijk het zo helder en nauwkeurig mogelijk overbrengen van de onderliggende data. En daar schort het bij ronde figuren vaak aan! Een groot nadeel is bijvoorbeeld dat ons brein heel slecht is om verschillen in oppervlakte tussen ronde vormen waar te nemen. Ook wordt het oppervlak groter naarmate de afstand tot het middelpunt toeneemt, wat voor vervorming zorgt bij bijvoorbeeld een cirkelvormig staafdiagram. 

Cirkelvormige figuren zijn daarom vooral geschikt voor meer kwalitatieve visualisaties. Een taartdiagram die laat zien dat 1 of 2 groepen duidelijk in de minderheid zijn (het exacte aantal doet er niet precies toe). Een andere toepassing is het tonen van tijd- of seizoensgebonden patronen in de data, waarbij ieder seizoen als een nieuw ring in de cirkel wordt weergeven. Ook hier is een ronde plot echter niet altijd geschikt: bij teveel ringen worden de buitenste ringen vele malen groter dan de binnenste ringen en zullen de plot gaan overheersen. 

Een mooie toepassing vond ik de cirkelvormige heatmap om te bekijken of en hoe mijn lichaam verandert gedurende de menstruatiecyclus.

Tijd- of seizoensgebonden trends
Het weergeven van een seizoensgebonden patroon kan op verschillende manier, afhankelijk van de overige trends in de data. Als de gemiddelde waarde over langere tijd stabiel is, zoals bij het meten van de lichaamstemperatuur, kan simpelweg de absoute waarde over de gehele cyclus uitgezet worden (Figuur 1). Als er echter sprake is van een trend over langere tijd, bijvoorbeeld in het geval van mijn gewicht die (slik...) over tijd met zo’n 5 kilo is toegenomen dan zegt de absolute waarde niets meer over de relatie tot de periode in de cyclus. In zo’n geval werkt het beter om te corrigeren voor de trend door bijvoorbeeld het voortschrijdende gemiddelde over een langere periode of het gemiddelde voor iedere cyclus te berekenen. Door  deze waarde van de werkelijke waarde af te trekken (additief model) of de verhouding van de werkelijke waarde tot deze trendwaarde te nemen (multiplicatief model) zou je alsnog een (sterk) patroon moeten kunnen waarnemen.


Temperatuur en de menstruatiecyclus
Gewicht en de menstruatiecyclus
Ademfrequentie en de menstruatiecyclus
Hartslagvariabiliteit en de menstruatiecylus
Hoofdpijn en de menstruatiecyclus


