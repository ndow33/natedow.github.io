---
layout: post
title: The goldrush continues
---

# A quick story about prospecting...

Picture this: you're a young carpenter living in California in 1848. You've moved to the rugged Sierra-Nevadas from New Mexico and are now working to help build a water-powered sawmill for a Swiss fellow. One day as you're going about your work, you notice a sparkle in the river. Upon taking a closer look, you realize what you've found: GOLD!!! 

Following the discovery of gold, the famous California Gold-Rush of 1849 ensued. That year, California's non-native population went from less than 1000 to over 100,000 filling the state with prospectors who were hopeful that they too might strike gold. Although the frenzy of the gold-rush has come and gone, the pursuit of “gold” continues today in a different form.

Today, instead of prospecting for literal gold, businesses prospect for people. For example, in sales, getting in front of the right person is paramount to success. Some of the qualities that the “right person” has include a problem your product can solve, authorization to buy, and budget. Much like gold, these people can be difficult to find. In fact, many companies have full-time employees whose entire job is to identify who these people are and reach out to them in an effort to get them to learn more. 

This process of finding and reaching out to the right people is actually called prospecting (you understand the analogy of the gold-rush now, don’t you). 

## What are sequences?

How does one find the right person? A sequence (also referred to as a cadence) is a plan of attack to do just that. It can include emails, phone calls, LinkedIn messages, and any other types of communication (including telegrams I suppose). 

Now you might be asking yourself, “how do you know so much about this?”. Well, it’s my job. So, I took this opportunity of learning about data analysis and visualization to create a useful report for me and my team. 

The question I wanted to answer was this: which sequences that include emails have the best reply rates? The better the reply rates, the better chance we have of talking with someone. The better chance we have of talking with someone, the better chance we have of finding the right person.

## The Data

[The data](https://github.com/ndow33/ndow33.github.io/blob/master/lambda_unit1_build/USE_2user-sequences-report-12_01_2019-02_22_2020%20-%20USE_user-sequences-report-12_01_2019-02_22_2020.csv) I decided to use came entirely from my sales team and is comprised of over 55,000 emails sent out across 26 different sequences. Each sequence has different messaging, timing, and other tasks associated with the emails (such as phone calls and LinkedIn messages), but for this analysis, we will be focusing on email open rates, email reply rates, and a metric I call the "true" reply rate.

## Visual 1: Sequences by Open Rates

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/50/#/" height="750" width="150%"></iframe>

This visualization shows the sequences by open rate. Each sequence has been used to send at least 100 emails. The blue line that goes across the bars represents the average open rate across all sequences. Now we can clearly see which sequences outperformed the average as well as which sequences had the best open rate in descending order from best to worst.

## Insights

What stood out most to me most is that the majority of our sequences are at or above the 30% open rate threshold the sequence 

## Visual 2: Sequences by Reply Rate

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/14/#/" height="750" width="150%"></iframe>

This visualization shows the sequences by reply rate. Each sequence has been used to send at least 100 emails. The blue line that goes across the bars represents the average reply rate across all sequences. Now we can clearly see which sequences outperformed the average as well as which sequences had the best reply rate in descending order from best to worst.

## Insights

Perhaps the most impactful insight that I gained from this analysis was just how effective the “US SDR - Referral Sequence - Q120” is. With a reply rate of nearly 14%, it nearly doubles the reply rate of the next closest sequence and more than quadruples the average reply rate of just under 3%. This sequence includes both phone calls and emails, but what sets this sequence apart from the others is the fact that the people who are contacted through it are referred to us by people within their organization. To me, this shows just how effective asking for a reference can be and will definitely be something that I discuss with my team. 

## Visual 3: Open Rates vs. Reply Rates

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/78/#/" height="750" width="150%"></iframe>

## Insights

## Visual 4: The "True" Reply Rate

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/32/#/" height="750" width="150%"></iframe>

## Insights

## Emails Sent vs. Reply Rate

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/97/#/" height="750" width="150%"></iframe>

## Insights

## Thanks!

Well, that’s all I have for now. I appreciate you taking the time to read through this post! If you have any questions or just want to connect, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/nathan-dow-42a846148/)! To see other visualizations that I'll be sharing with my team for other sequence related insights, click [here](https://ndow33.github.io/2020-03-07-Sequence-visualizations/).


