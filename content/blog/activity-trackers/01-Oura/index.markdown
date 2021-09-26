---
title: "Oura Ring"
weigth: 1
subtitle: "A ring that measures sleep, activity and readiness"
excerpt: "A post about the Oura Ring"
date: 2021-09-27
draft: true
---

## What is the Oura Ring

The Oura ring measures xxxx etc.

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


