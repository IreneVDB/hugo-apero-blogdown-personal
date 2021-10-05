---
title: "Ōura Ring"
weight: 1
subtitle: "A ring that measures sleep, activity and readiness"
excerpt: "What is the Ōura Ring and what can you do with the data? An overview of my experiences with the Ōura Ring for tracking **Sleep**, **Activity** and **Readiness**. Accompanied by instructions and visualizations on how to access and analyze your Ōura Ring data in R"
date: 2021-09-26
draft: false
categories: [Sleep, Activity]

---

<link href="{{< blogdown/postref >}}index_files/panelset/panelset.css" rel="stylesheet" />

<script src="{{< blogdown/postref >}}index_files/panelset/panelset.js"></script>

## What is the Ōura Ring?

A pretty piece of jewelry on the outside with a variety of sensors hidden on the inside\! The [Ōura Ring](https://oura.com) is a **Sleep** and **Activity** tracker that measures heart and breathing rate, skin temperature, and motion. Without any effort, and with very little non-wear time, I have already collected a wealth of data over **614** days. Here, you can read all about my experiences collecting, analyzing and visualizing my Ōura Ring data\!

## How to get your data?

All daily activity and nightly sleep data are stored on your (free) Ōura cloud account. Both the Ōura cloud platform and the Ōura app have some nice features to view daily, weekly or monthly trends in your data. However, if you (like me 😄) want to analyze and visualize your own data, you can get the data in your own hands by either:

1.  Export your data as a`.csv` or `.json` file from the Oura cloud account; or
2.  Connect through Ōura cloud API using a *personal access token*.

The available data from the Ōura Ring is summarized below. A detailed description of all measured parameters can also be found in the Ōura Ring [API documentation](https://cloud.ouraring.com/docs/).

## Data for Sleep and Activity Tracking

In the below panels you see an overview of all numeric data values measured with the Ōura Ring during sleep (Fig. <a href="#fig:SleepMetrics">1</a>) or daily activity (Fig. <a href="#fig:ActivityMetrics">2</a>).

<div class="panelset">

<div class="panel">

## Sleep

<div class="figure">

<img src="{{< blogdown/postref >}}index_files/figure-html/SleepMetrics-1.png" alt="\label{fig:SleepMetrics}Distribution of daily sleep metrics measured wih the Ōura Ring, including the durations of various sleep phases (**Rem**, **Deep** and **Light**), the total sleep time (**Total**), the time in bed (**Duration**), the time awake (**Awake**), the time to fall asleep (**Onset Latency**), as well as the percentage of time asleep (**Effciency**) and the percentag of time that motion is detected (**Restless**). In addition, the average breathing rate (**Breath Average**), the average and lowest heart rate (**Hr Average** and **Hr Lowest**), the average heart rate variability (**Rmssd**) and the average skin temperature deviation (**Temperature Deviation**) are provided." width="720" />

<p class="caption">

Figure 1: Distribution of daily sleep metrics measured wih the Ōura Ring, including the durations of various sleep phases (**Rem**, **Deep** and **Light**), the total sleep time (**Total**), the time in bed (**Duration**), the time awake (**Awake**), the time to fall asleep (**Onset Latency**), as well as the percentage of time asleep (**Effciency**) and the percentag of time that motion is detected (**Restless**). In addition, the average breathing rate (**Breath Average**), the average and lowest heart rate (**Hr Average** and **Hr Lowest**), the average heart rate variability (**Rmssd**) and the average skin temperature deviation (**Temperature Deviation**) are provided.

</p>

</div>

</div>

<div class="panel">

## Activity

<div class="figure">

<img src="{{< blogdown/postref >}}index_files/figure-html/ActivityMetrics-1.png" alt="\label{fig:ActivityMetrics}Distribution of all daily activity metrics measured wih the Ōura Ring." width="720" />

<p class="caption">

Figure 2: Distribution of all daily activity metrics measured wih the Ōura Ring.

</p>

</div>

</div>

</div>

## Sleep, Activity and Readiness Scores

Based on the Sleep and Activity metrics, the Ōura Ring calculates a daily **Sleep**, **Activity** and **Readiness** score. In Figure <a href="#fig:TotalScores">3</a>, you see the distribution of my scores over 614 days, whereas the panels underneath show the distribution in the individual scores used to calculate the total scores.

<div class="figure">

<img src="{{< blogdown/postref >}}index_files/figure-html/TotalScores-1.png" alt="\label{fig:TotalScores}Distribution of daily Sleep, Activity and Readiness Scores measured wih the Ōura Ring." width="720" />

<p class="caption">

Figure 3: Distribution of daily Sleep, Activity and Readiness Scores measured wih the Ōura Ring.

</p>

</div>

<div class="panelset">

<div class="panel">

## Sleep

<div class="figure">

<img src="{{< blogdown/postref >}}index_files/figure-html/SleepScores-1.png" alt="\label{fig:SleepScores}The daily Sleep Score is based on the individual scores for the total amount of sleep (**Total**), the amount of **REM** and **Deep** sleep, sleep **Efficiency**, the time it takes to fall asleep (**Latency**), the amount of restlessness (**Disturbances**) and the sleep timing (**Alignment**)." width="720" />

<p class="caption">

Figure 4: The daily Sleep Score is based on the individual scores for the total amount of sleep (**Total**), the amount of **REM** and **Deep** sleep, sleep **Efficiency**, the time it takes to fall asleep (**Latency**), the amount of restlessness (**Disturbances**) and the sleep timing (**Alignment**).

</p>

</div>

</div>

<div class="panel">

## Activity

<div class="figure">

<img src="{{< blogdown/postref >}}index_files/figure-html/ActivityScores-1.png" alt="\label{fig:ActivityScores}The daily Activity Score is based on the scores for." width="720" />

<p class="caption">

Figure 5: The daily Activity Score is based on the scores for.

</p>

</div>

</div>

<div class="panel">

## Readiness

<div class="figure">

<img src="{{< blogdown/postref >}}index_files/figure-html/ReadinessScores-1.png" alt="\label{fig:ReadinessScores}The daily Readiness Score is based on the scores for xxx as well as xxx from sleep (fig x)." width="720" />

<p class="caption">

Figure 6: The daily Readiness Score is based on the scores for xxx as well as xxx from sleep (fig x).

</p>

</div>

</div>

</div>

## Daily Timestamps

<div class="figure">

<img src="{{< blogdown/postref >}}index_files/figure-html/SleepTimes-1.png" alt="\label{fig:SleepTimes} The Ōura Ring data includes timestamps for the time at which you go to bed (**Bedtime Start**), the time that you get up (**Bedtime End**) and the time in the middle of your sleep (**Midpoint**),used to calculate the Alignment score for sleep timing." width="720" />

<p class="caption">

Figure 7:  The Ōura Ring data includes timestamps for the time at which you go to bed (**Bedtime Start**), the time that you get up (**Bedtime End**) and the time in the middle of your sleep (**Midpoint**),used to calculate the Alignment score for sleep timing.

</p>

</div>

### Daily Time Series

## Conclusion

The Ōura Ring stands out for it’s **data accessibility** and the **ease of wearing**.

Although the Ōura Ring isn’t cheap, it’s fashionable look and compact size, make the Ōura Ring easily worn day and night, collecting a wealth a data with little to no missing data points\! The Ōura ring fully charges in about 1-2 hours and lasts for almost 4 days. As a sleep tracker, the Ōura Ring is great for tracking your sleep pattern and nightly body functions. However, the Ōura Ring is not very accurate in sleep staging, particularly in differentiating laying down from actual sleeping.

### Ōura Ring - Pros:

  - Good data visualization options in app and cloud platform.
  - Data is fully accessible through file export or API.
  - No bluetooth connection during inactivity or sleep.
  - Can be worn day and night without noticing.
  - Little “non-wear” time due to charging.
  - Fashionable look.

### Ōura Ring - Cons:

  - Not cheap (price starts at $299).
  - Not very accurate in sleep stage detection (certainly not able to differentiate laying still from actual sleeping).
  - Be careful; you don’t want to lose or damage the ring\!
  - Skin temperature and breathing rate data are only available as a nightly average.
  - Meditation data is not available.

## Resources

<svg aria-hidden="true" role="img" viewBox="0 0 496 512" style="height:1em;width:0.97em;vertical-align:-0.125em;margin-left:auto;margin-right:auto;font-size:inherit;fill:currentColor;overflow:visible;position:relative;"><path d="M165.9 397.4c0 2-2.3 3.6-5.2 3.6-3.3.3-5.6-1.3-5.6-3.6 0-2 2.3-3.6 5.2-3.6 3-.3 5.6 1.3 5.6 3.6zm-31.1-4.5c-.7 2 1.3 4.3 4.3 4.9 2.6 1 5.6 0 6.2-2s-1.3-4.3-4.3-5.2c-2.6-.7-5.5.3-6.2 2.3zm44.2-1.7c-2.9.7-4.9 2.6-4.6 4.9.3 2 2.9 3.3 5.9 2.6 2.9-.7 4.9-2.6 4.6-4.6-.3-1.9-3-3.2-5.9-2.9zM244.8 8C106.1 8 0 113.3 0 252c0 110.9 69.8 205.8 169.5 239.2 12.8 2.3 17.3-5.6 17.3-12.1 0-6.2-.3-40.4-.3-61.4 0 0-70 15-84.7-29.8 0 0-11.4-29.1-27.8-36.6 0 0-22.9-15.7 1.6-15.4 0 0 24.9 2 38.6 25.8 21.9 38.6 58.6 27.5 72.9 20.9 2.3-16 8.8-27.1 16-33.7-55.9-6.2-112.3-14.3-112.3-110.5 0-27.5 7.6-41.3 23.6-58.9-2.6-6.5-11.1-33.3 2.6-67.9 20.9-6.5 69 27 69 27 20-5.6 41.5-8.5 62.8-8.5s42.8 2.9 62.8 8.5c0 0 48.1-33.6 69-27 13.7 34.7 5.2 61.4 2.6 67.9 16 17.7 25.8 31.5 25.8 58.9 0 96.5-58.9 104.2-114.8 110.5 9.2 7.9 17 22.9 17 46.4 0 33.7-.3 75.4-.3 83.6 0 6.5 4.6 14.4 17.3 12.1C428.2 457.8 496 362.9 496 252 496 113.3 383.5 8 244.8 8zM97.2 352.9c-1.3 1-1 3.3.7 5.2 1.6 1.6 3.9 2.3 5.2 1 1.3-1 1-3.3-.7-5.2-1.6-1.6-3.9-2.3-5.2-1zm-10.8-8.1c-.7 1.3.3 2.9 2.3 3.9 1.6 1 3.6.7 4.3-.7.7-1.3-.3-2.9-2.3-3.9-2-.6-3.6-.3-4.3.7zm32.4 35.6c-1.6 1.3-1 4.3 1.3 6.2 2.3 2.3 5.2 2.6 6.5 1 1.3-1.3.7-4.3-1.3-6.2-2.2-2.3-5.2-2.6-6.5-1zm-11.4-14.7c-1.6 1-1.6 3.6 0 5.9 1.6 2.3 4.3 3.3 5.6 2.3 1.6-1.3 1.6-3.9 0-6.2-1.4-2.3-4-3.3-5.6-2z"/></svg> Code to collect, analyze and visualize my Ōura Ring data on [Github](https://github.com/IreneVDB/OuraRing)

And more plots with links here as tiny figures
