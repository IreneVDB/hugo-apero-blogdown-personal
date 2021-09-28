---
title: "Ōura Ring"
weigth: 1
subtitle: "A ring that measures sleep, activity and readiness"
excerpt: "What is the Ōura Ring and what can you do with the data? An overview my experiences with the Ōura Ring for tracking **Sleep**, **Activity** and **Readiness**. Accompanied by instructions and visualizations on how to access and analyze your Ōura Ring data in R"
date: 2021-09-26
draft: false
---

<img src="featured-Oura.png" width="50%" style="margin-left:25%; margin-right:25%; border-radius:5%"/>

## What is the Ōura Ring?

A pretty piece of jewelry on the outside with a variety of sensors hidden on the inside! The [Ōura Ring](https://oura.com) is both a **Sleep** and **Activity** tracker that measures heart and breathing rate, skin temperature, and motion. In the Ōura Ring app you can view your daily **Sleep**, **Activity** and **Readiness** scores as well as *personalized* recommendations about your sleep pattern, recovery, or workout intensity. <p>

The Ōura Ring app integrates with the Apple or Samsung Health app and can import your training activity from various third party workout apps. You can also use the Ōura Ring app to take a guided or unguided **mediation** session. When the meditation session is longer than 10 minutes, both heart rate, heart rate variability (HRV) and skin temperature will be measured. Although the effects of the meditation session on these body functions are displayed in the Ōura Ring app afterwards, the raw meditation data is not accessible for further analysis.

## Pros and Cons of the Ōura Ring

For me, the Ōura Ring stands out for it's **data accessibility** and the **ease of wearing**. Except for the meditation data, all daily activity and nightly sleep data is stored and accessible through the Ōura cloud platform. In addition, the Ōura Ring [API documentation](https://cloud.ouraring.com/docs/) provides a detailed and complete description of all parameters and their weights in the device scoring algorithms. Nonetheless, it is good to know that only aggregated data is accessible, either as a single value or, for a few metrics, aggregated in 1 or 5 minute intervals (See <a href="#how-to-data">0.3</a>)

Although the Ōura Ring isn't cheap, it's fashionable look and compact size, make the Ōura Ring easily worn day and night, collecting a wealth a data with little to no missing data points! The Ōura ring fully charges in about 1-2 hours and lasts for almost 4 days. For use as a sleep tracker, the Ōura Ring is great to keep track of your sleep pattern as well as your resting heart rate, mean HRV and body temperature during the night. The Ōura Ring is, however, not very accurate in sleep staging and differentiating laying down from actual sleeping. 

### Ōura Ring - Pros:

- Good data visualization options in app and cloud platform.
- Data is fully accessible through file export or API.
- No bluetooth connection during inactivity or sleep.
- Can be worn day and night without noticing.
- Little "non-wear" time due to charging.
- Fashionable look.

### Ōura Ring - Cons:

- Not cheap (price starts at $299).
- Not very accurate in sleep stage detection (certainly not able to differentiate laying still from actual sleeping).
- Be careful; you don't want to lose or damage the ring!
- Skin temperature and breathing rate data are only available as a nightly average.
- Meditation data is not available.

## How to get your data from the Ōura Ring? {#how-to-data}

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


