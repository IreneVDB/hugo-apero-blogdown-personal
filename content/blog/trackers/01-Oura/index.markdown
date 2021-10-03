---
title: "Ōura Ring"
weigth: 1
subtitle: "A ring that measures sleep, activity and readiness"
excerpt: "What is the Ōura Ring and what can you do with the data? An overview of my experiences with the Ōura Ring for tracking **Sleep**, **Activity** and **Readiness**. Accompanied by instructions and visualizations on how to access and analyze your Ōura Ring data in R"
date: 2021-09-26
draft: false
---



## What is the Ōura Ring?

A pretty piece of jewelry on the outside with a variety of sensors hidden on the inside! The [Ōura Ring](https://oura.com) is both a **Sleep** and **Activity** tracker that measures heart and breathing rate, skin temperature, and motion to calculate your daily **Sleep**, **Activity** and **Readiness** scores. <p>

The Ōura Ring app integrates with the Apple or Samsung Health app as well as various third party workout apps. You can also start a guided or unguided **mediation** session in the Ōura Ring app while the Ōura Ring records your heart rate, heart rate variability (HRV) and skin temperature. 

## How to get the Ōura Ring's data?

All daily activity and nightly sleep data are stored on your (free) Ōura cloud account. Both the Ōura cloud platform and the Ōura app have some nice features to view daily, weekly or monthly trends in your data. However, if you (like me 😄) want to analyze and visualize your own data, there are several ways to get the data in your own hands:

  1. Export your data as a`.csv ` or `.json` file from the Oura cloud account; or
  2. Connect through Ōura cloud API using a *personal access token*.

Note that only aggregated data is accessible, either as a single value or, for a few metrics, as average over 1 or 5 minute intervals.

## What does the Oura Ring measure?

The Ōura Ring [API documentation](https://cloud.ouraring.com/docs/) provides a detailed description of all measured parameters. The data from the Ōura Ring includes:
- Daily Sleep, Activity and Readiness Scores.
- Daily (or nightly) aggregates (e.g., total sleep hours, step counts, or average breathing rate while asleep)
- Daily time stamps (e.g., the time you go to bed, fall asleep or get up)
- Daily or nightly time series (as average per 1 or 5 minute intervals)

### Daily Sleep, Activity or Readiness Scores

Every day the Ōura Ring gives a score for your Sleep, Activity and Readiness. In Figure \@ref(fig:TotalScores_dim), you see the distribution of my scores over 610 days of measurement.

<div class="figure">
<img src="{{< blogdown/postref >}}index_files/figure-html/TotalScores_dim-1.png" alt="Some caption for this plot" width="672" />
<p class="caption">(\#fig:TotalScores_dim)Some caption for this plot</p>
</div>

Each score is calculated based on the following scores summarized in the panels below:

{{< panelset class="greetings" >}}
{{< panel name="Sleep" >}}

<img src="{{< blogdown/postref >}}index_files/figure-html/Sleep_Scores-1.png" width="672" />

{{< /panel >}}
{{< panel name="Activity" >}}

<img src="{{< blogdown/postref >}}index_files/figure-html/Activity_Scores-1.png" width="672" />

{{< /panel >}}
{{< panel name="Readiness" >}}

<img src="{{< blogdown/postref >}}index_files/figure-html/Readiness_Scores-1.png" width="672" />

{{< /panel >}}
{{< /panelset  >}}

### Daily aggregates

And here an overview of _all_ available daily metrics measured with the Ōura Ring.

{{< panelset class="greetings" >}}

{{< panel name="Sleep" >}}

<img src="{{< blogdown/postref >}}index_files/figure-html/Sleep_metrics-1.png" width="672" />

{{< /panel >}}
{{< panel name="Activity" >}}

<img src="{{< blogdown/postref >}}index_files/figure-html/Activity_metrics-1.png" width="672" />

{{< /panel >}}
{{< /panelset  >}}


### Timestamps

### Daily time series




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




