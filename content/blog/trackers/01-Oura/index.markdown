---
title: "Ōura Ring"
weigth: 1
subtitle: "A ring that measures sleep, activity and readiness"
excerpt: "What is the Ōura Ring and what can you do with the data? An overview of my experiences with the Ōura Ring for tracking **Sleep**, **Activity** and **Readiness**. Accompanied by instructions and visualizations on how to access and analyze your Ōura Ring data in R"
date: 2021-09-26
draft: false
---

<img src="featured-Oura.png" width="50%" style="margin-left:25%; margin-right:25%; border-radius:5%"/>

## What is the Ōura Ring?

A pretty piece of jewelry on the outside with a variety of sensors hidden on the inside! The [Ōura Ring](https://oura.com) is both a **Sleep** and **Activity** tracker that measures heart and breathing rate, skin temperature, and motion to calculate your daily **Sleep**, **Activity** and **Readiness** scores. <p>

The Ōura Ring app integrates with the Apple or Samsung Health app as well as various third party workout apps. You can also start a guided or unguided **mediation** session in the Ōura Ring app while the Ōura Ring records your heart rate, heart rate variability (HRV) and skin temperature. 

## How to get your data from the Ōura Ring?

All daily activity and nightly sleep data are stored on your (free) Ōura cloud account. Both the Ōura cloud platform and the Ōura app have some nice features to view daily, weekly or monthly trends in your data. However, if you (like me 😄) want to analyze and visualize your own data, there are several ways to get the data in your own hands.

In the below panels I discuss two approaches to get your Ōura Ring for further analysis in R: 
  1. Export your data as a`.csv ` or `.json` file from the Oura cloud account; and
  2. Connect through Ōura cloud API using a *personal access token*.

I should not that only aggregated data is accessible, either as a single value or, for a few metrics, as average over 1 or 5 minute intervals (See [What does the Oura Ring measure?](metrics))

{{< panelset class="greetings" >}}
{{< panel name="Export data file" >}}

From your Ōura cloud account you can download data as:
- `.csv`: Under **<Trends>** select the date range, click **<Download Data>** and choose all or a selection of values.
- `.json`: Go to **<My Account>** and click the **<Download>** button.

Both `.csv` and `.json` files are easily imported into R:

```r
Oura_csv <- read.csv("path/to/file/filename.csv", sep=",")
Oura_json <- jsonlite::fromJSON("path/to/file/filename.json")
```

{{< /panel >}}
{{< panel name="Connect with API" >}}
  jkhkjhkjh
{{< /panel >}}
{{< /panelset  >}}

## DOet deze panelset het wel?

{{< panelset class="greetings" >}}
{{< panel name="Plot" >}}

<img src="{{< blogdown/postref >}}index_files/figure-html/plot-1.png" width="672" />

{{< /panel >}}
{{< panel name="Code" >}}


```r
plot(pressure)
```

{{< /panel >}}
{{< /panelset  >}}

## What does the Oura Ring measure? (#metrics)

The Ōura Ring [API documentation](https://cloud.ouraring.com/docs/) provides a detailed description of all measured parameters.

Here some beeswarm plots and a summary of all the metrics.

<img src="{{< blogdown/postref >}}index_files/figure-html/plot2-1.png" width="672" />

## Ōura Ring: Pros and Cons

The Ōura Ring stands out for it's **data accessibility** and the **ease of wearing**. 

Although the Ōura Ring isn't cheap, it's fashionable look and compact size, make the Ōura Ring easily worn day and night, collecting a wealth a data with little to no missing data points! The Ōura ring fully charges in about 1-2 hours and lasts for almost 4 days. As a sleep tracker, the Ōura Ring is great for tracking your sleep pattern and nightly body functions. However, the Ōura Ring is not very accurate in sleep staging, particularly in differentiating laying down from actual sleeping. 

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


## Some text

And here I am using my own lungs like a sucker. __How is education supposed to make me feel smarter?__ *Besides, every time I learn something new, it pushes some old stuff out of my brain.* Remember when I took that home winemaking course, and I forgot how to drive?

Marge, just about everything's a sin. 
* You know, the one with all the well meaning rules that don't work out in real life, uh, Christianity.
* Your questions have become more redundant and annoying than the last three "Highlander" movies.
* D'oh. 


