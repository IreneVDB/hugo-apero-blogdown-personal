---
title: "Oura Ring"
weigth: 1
subtitle: "A ring that measures sleep, activity and readiness"
excerpt: "A post about the Oura Ring - but now in another series"
date: 2021-09-26
draft: false
---


<img src="featured-Oura.png" width="50%" style="margin-left:25%; margin-right:25%; border-radius:5%"/>

## What is the Oura Ring?

<img src="https://play-lh.googleusercontent.com/-9sv7pGewA5xDhZttAWNm8N1p4iGuPctvej8kwBaLs0wm8bweNZGYkYTwcSTxkVq6l8-=s360" width="10%" style="float:left; border-radius:10%; margin-right:5px"/>

A pretty piece of jewelry on the outside with a variety of sensors hidden on the inside! These sensors measure heart rate, heart rate variability, breathing rate, skin temperature, motion and step count. Because of the [Oura Ring](https://oura.com)'s size and looks, you can collect a wealth of data while wearing the ring day and night.


De Oura Ring is ook een slaap tracker: aan de hand van je hartslag en beweging bepaalt de ring het tijdstip waarop je in en uit bed gaat, in slaap valt en wakker wordt, en zelfs van de fase van je slaap. Uit onderzoek is gebleken dat de Oura ring enerzijds goed slaap, ofwel de tijd die je in bed ligt, kan detecteren (gevoeligheid van 96%), maar anderzijds minder goed wakkere momenten van echte slaap kan onderscheiden (specificiteit van 48%) of slaapfases kan classificeren (65%, 51% en 61% overeenkomst met lichte, diepe, en REM slaap, respectievelijk) [1].
 
Via de app worden deze gegevens gebruikt om je inzicht te geven in je fysieke gesteldheid door middel van een slaapscore, een activiteitscore en een algehele paraatheid (‘readiness’) score. Om deze scores van meer waarde te laten zijn, kun je via de app je trainingen toevoegen, zowel handmatig als door een koppeling met je favoriete trainingsapp. Ook geeft de app de mogelijkheid om begeleide en onbegeleide ontspanningsoefeningen te doen.



## How to get your Data?

You can get your data via API, FTTT or exported as json or csv file. See the tabs below for more info and sample code.

{{< panelset class="greetings" >}}
{{< panel name="Hello! :wave:" >}}
  hello
{{< /panel >}}
{{< panel name="Goodbye :dash:" >}}
  goodbye
{{< /panel >}}
{{< /panelset  >}}

## What does the Oura Ring measure?

Here some beeswarm plots and a summary of all the metrics.

<img src="{{< blogdown/postref >}}index_files/figure-html/plot-1.png" width="672" />

## Data Visualizations

And more plots with links here as tiny figures

![figure1]("featured-Oura.png")

## Conclusion

Pros and cons of the OUra Ring in a table?

## Resources

A list:
1. jhgkjg
2. kjhkjh
3. kjghkjh


```r
library(tidyverse)
```

```
## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.0 ──
```

```
## ✓ ggplot2 3.3.2     ✓ purrr   0.3.4
## ✓ tibble  3.0.3     ✓ dplyr   1.0.2
## ✓ tidyr   1.1.2     ✓ stringr 1.4.0
## ✓ readr   1.3.1     ✓ forcats 0.5.0
```

```
## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
## x dplyr::filter() masks stats::filter()
## x dplyr::lag()    masks stats::lag()
```

```r
library(palmerpenguins)
```


```r
ggplot(data = penguins, aes(x = flipper_length_mm)) +
  geom_histogram(aes(fill = species), alpha = 0.5, position = "identity") +
  scale_fill_manual(values = c("darkorange","darkorchid","cyan4"))
```

```
## `stat_bin()` using `bins = 30`. Pick better value with `binwidth`.
```

```
## Warning: Removed 2 rows containing non-finite values (stat_bin).
```

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-2-1.png" width="672" />

## Some text

And here I am using my own lungs like a sucker. __How is education supposed to make me feel smarter?__ *Besides, every time I learn something new, it pushes some old stuff out of my brain.* Remember when I took that home winemaking course, and I forgot how to drive?

Marge, just about everything's a sin. 
* You know, the one with all the well meaning rules that don't work out in real life, uh, Christianity.
* Your questions have become more redundant and annoying than the last three "Highlander" movies.
* D'oh. 


