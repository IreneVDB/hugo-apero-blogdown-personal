---
title: "Rescue Time"
weight: 2
subtitle: "An app to track your computer and mobile phone usage"
excerpt: "The RescueTime app is a **productivity** tracker that you can install on your computer and mobile devices. Here, you'll read about my experiences with the RescueTime app and how you can get the most out of your data!"
date: 2021-10-24
draft: true
categories: [Habits, Productivity, RescueTime]

---

<style>body {text-align: justify}</style>

## What is the RescueTime app?

I love apps and trackers that *continuously* gather data while you don’t have to do anything\! The RescueTime app is such an app. You simply install the RescueTime app on your mobile phone(s), tablet(s) and/or computer(s) and the app tracks *when* and for *how long* you use the device. When installed on your laptop or desktop computer, the RescueTime app also tracks *what* you were doing and how *productive* your activity has been.

This way, I have been collecting data about my productivity for already **460** days. On your mobile devices the app needs to be opened in the background, which means that when you accidentally close the app, it won’t track\! So far, I have collected data on my mobile devices for **354** days.

## How to get your data?

There are several ways to get your RescueTime data. The easiest way may be on your [RescueTime account](https://www.rescuetime.com), where you can find a link to “Download your data archive” under the “Your data” heading in the sidebar of the “Account Settings” page. When you click this link, you can generate a `.csv` file which lists the number of minutes for each activity per hour of the day for your entire logging history.

Alternatively, you can get your data using the [RescueTime API](https://www.rescuetime.com/anapi/setup/documentation). In contrast to the data archive downloaded from your RescueTime account, the Rescue Time API, unfortunately, does not allow you to retrieve data from more than 3 months ago if you don’t have a Premium account. On the other hand, the data from the RescueTime API can be summarized in chunks with a minimum size of 5 minutes and also includes **productivity metrics**.

## Productivity Metrics

The productivity metrics are assigned as to each activity and categorized as *Very Distracting*, *Distracting*, *Neutral*, *Productive* and *"Very Productive* (Figure 1). The productivity score is of course a bit arbitrary as you can be very productive when visiting a webshop, whereas you can perform completely irrelevant work using a text editor. To get a better insight in your productivity, you can manually adjust the productivity metrics for every activity in your RescueTime account.

RescueTime\_plots\[\[Productivity\]\]\[\[“pie”\]\]
Figure 1: A bar chart with the productivity metrics as relative %
RescueTime\_plots\[\[Productivity\]\]\[\[“beeswarm”\]\]
Figure 2: A beeswarm with the disribution of productivity metrics as hours per day
Figure 3: A bar chart with the productivity pe rhour of day

## Computer vs. Mobile device

Besides the productivity metrics, RescueTime also allows you to track *when* and for *how long* you use your computer or mobile device(s). It should, however, be noted that the RescueTime app on your mobile device cannot track which app or program is being used. For me, any time spent on my tablet or mobile phone is categorized as “iOS device” and assigned a **Very Distracing** productivity score.

Using the RescueTime API, you can get a summary of your activity data in chunks of 5 minutes. With this data, I visualized the average time spent on my laptop vs. my mobile devices across the days of the week (@ref(fig:Laptop\_vs\_Mobile)). In addition, the heatmaps in Figure @ref(fig:HM\_screentime) and Figure @ref(fig:HM\_mobile) show the time spent on either my laptop or mobile devices across the entire logging period (460 days).

<div class="panelset">

<div class="panel">

### Screen Time

</div>

<div class="panel">

### Mobile device usage

</div>

</div>

## Categories

All activities are categorized into 11 main categories which are further divided into \~60 sub-categories (Figure xxx). You can manually adjust the categorization in your RescueTime account, which is especially usefull for frequently used applications that would otherwise be left ‘uncategorized’ (and assigned a ‘neutral’ productivity score).

Figure xxx shows the average time per day spent in the 11 top-level categories.

## Activities

Lastly, the RescueTime app on your desktop computer tracks the time spent on each individual application, website or activity. The Treemap in Figure xxx shows that **R Studio** is clearly my favorite application\!

<img src="/img/app_logos/RescueTime.png" width="10%" style="float:left; border-radius:10%; margin:5px;"/>

## Conclusion

The RescueTime app allows you to freely and silently gather a wealth of data about your computer and phone use. Although your RescueTime account already allows you to view your statistics and create reports in various ways, the best part of the RescueTime app - to me 😄 - is the accessibility of your own data. However, when using the (well-documented) RescueTime API, you need to make sure to download and store your data at least every 3 months.

If you want to improve your productivity, the RescueTime app offers various tools to, for example, set goals or time limits, or even block certain (distracting) applications or websites. A Premium subscription offers even more tools to potentially enhance your productivity, but comes at a monthly cost of $12 (or $78 annually) which, for me, is not worth the merits.

### RescueTime - Pros:

  - Data about computer and mobile device usage are continuously being monitored
  - All data is (freely) accesible without need for Premium subscription.
  - You can install the RescueTime app on multiple computers as well as your mobile phone(s) or tablet(s).
  - You can automate your data collection using the (well-documented) RescueTime API.
  - You can analyze and visualize various activity and productivity metrics, and generate reports, on your RescueTime account.

### RescueTime - Cons:

  - The mobile RescueTime app only tracks time and does not log which programs are used.
  - When your mobile device(s) have the same OS you won’t be able to differatiate between the time on each device as all activities are categorized as, for example, “iOS device”.
  - For accurate use of the automatically assigned productivity metrics, a manual check or adjustment is needed.
  - Without the Premium account the RescueTime API only allows access to data from the last 3 months.

## Resources

  - <svg aria-hidden="true" role="img" viewBox="0 0 496 512" style="height:1em;width:0.97em;vertical-align:-0.125em;margin-left:auto;margin-right:auto;font-size:inherit;fill:currentColor;overflow:visible;position:relative;"><path d="M165.9 397.4c0 2-2.3 3.6-5.2 3.6-3.3.3-5.6-1.3-5.6-3.6 0-2 2.3-3.6 5.2-3.6 3-.3 5.6 1.3 5.6 3.6zm-31.1-4.5c-.7 2 1.3 4.3 4.3 4.9 2.6 1 5.6 0 6.2-2s-1.3-4.3-4.3-5.2c-2.6-.7-5.5.3-6.2 2.3zm44.2-1.7c-2.9.7-4.9 2.6-4.6 4.9.3 2 2.9 3.3 5.9 2.6 2.9-.7 4.9-2.6 4.6-4.6-.3-1.9-3-3.2-5.9-2.9zM244.8 8C106.1 8 0 113.3 0 252c0 110.9 69.8 205.8 169.5 239.2 12.8 2.3 17.3-5.6 17.3-12.1 0-6.2-.3-40.4-.3-61.4 0 0-70 15-84.7-29.8 0 0-11.4-29.1-27.8-36.6 0 0-22.9-15.7 1.6-15.4 0 0 24.9 2 38.6 25.8 21.9 38.6 58.6 27.5 72.9 20.9 2.3-16 8.8-27.1 16-33.7-55.9-6.2-112.3-14.3-112.3-110.5 0-27.5 7.6-41.3 23.6-58.9-2.6-6.5-11.1-33.3 2.6-67.9 20.9-6.5 69 27 69 27 20-5.6 41.5-8.5 62.8-8.5s42.8 2.9 62.8 8.5c0 0 48.1-33.6 69-27 13.7 34.7 5.2 61.4 2.6 67.9 16 17.7 25.8 31.5 25.8 58.9 0 96.5-58.9 104.2-114.8 110.5 9.2 7.9 17 22.9 17 46.4 0 33.7-.3 75.4-.3 83.6 0 6.5 4.6 14.4 17.3 12.1C428.2 457.8 496 362.9 496 252 496 113.3 383.5 8 244.8 8zM97.2 352.9c-1.3 1-1 3.3.7 5.2 1.6 1.6 3.9 2.3 5.2 1 1.3-1 1-3.3-.7-5.2-1.6-1.6-3.9-2.3-5.2-1zm-10.8-8.1c-.7 1.3.3 2.9 2.3 3.9 1.6 1 3.6.7 4.3-.7.7-1.3-.3-2.9-2.3-3.9-2-.6-3.6-.3-4.3.7zm32.4 35.6c-1.6 1.3-1 4.3 1.3 6.2 2.3 2.3 5.2 2.6 6.5 1 1.3-1.3.7-4.3-1.3-6.2-2.2-2.3-5.2-2.6-6.5-1zm-11.4-14.7c-1.6 1-1.6 3.6 0 5.9 1.6 2.3 4.3 3.3 5.6 2.3 1.6-1.3 1.6-3.9 0-6.2-1.4-2.3-4-3.3-5.6-2z"/></svg> Code to collect, analyze and visualize my RescueTime data on [Github](https://github.com/IreneVDB/RescueTime)
  - RescueTime [website](https://www.rescuetime.com)
  - RescueTime [API documentation](https://www.rescuetime.com/anapi/setup/documentation)
