---
layout: post
title: The goldrush continues
subtitle: A data visualization of prospecting
bigimg: /img/gold_scale.jpg
---

# A quick story about prospecting...

Picture this: you're a young carpenter living in California in 1848. You've moved to the rugged Sierra-Nevadas from New Mexico and are now working to build a water-powered sawmill for a Swiss fellow. One day as you're going about your work, you notice a sparkle in the river. Upon taking a closer look, you realize what you've found: GOLD!!! 

Following the discovery of gold, the famous California Gold-Rush of 1849 ensued. That year, California's non-native population went from less than 1000 to over 100,000 filling the state with prospectors who were hopeful that they too might strike gold. Although the frenzy of the gold-rush has come and gone, the pursuit of “gold” continues today in a different form.

Now, businesses prospect for people. For example, in sales, getting in front of the right person is paramount to success. Some of the qualities that the “right person” has include a problem your product can solve, authorization to buy, and budget. Much like gold, these people can be difficult to find. In fact, many companies have full-time employees whose entire job is to identify who these people are and reach out to them in an effort to get them to learn more. 

This process of finding and reaching out to the right people is actually called prospecting (you understand the analogy of the gold-rush now, don’t you). 

## What are sequences?

How does one find the right person? A sequence (also referred to as a cadence) is a plan of attack to do just that. It can include emails, phone calls, LinkedIn messages, and any other types of communication (including telegrams I suppose). 

Now you might be asking yourself, “how do you know so much about this?”. Well, it’s my job. So, I took this opportunity of learning about data analysis and visualization to create a useful report for me and my team. 

# My Question...

The question I wanted to answer was this: which sequences that include emails have the best open, reply, and "True" reply rates? The better these rates, the better chance we have of talking with someone. The better chance we have of talking with someone, the better chance we have of finding the right person.

## The Data

[The data](https://github.com/ndow33/ndow33.github.io/blob/master/lambda_unit1_build/USE_2user-sequences-report-12_01_2019-02_22_2020%20-%20USE_user-sequences-report-12_01_2019-02_22_2020.csv) I decided to use came entirely from my sales team and is comprised of over 55,000 emails sent out across 26 different sequences. Each sequence has different messaging, timing, and other tasks associated with the emails (such as phone calls and LinkedIn messages), but for this analysis, we will be focusing on email open rates, email reply rates, and a metric I call the "true" reply rate.

## Visual 1: Sequences by Open Rates

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/50/#/" height="750" width="150%"></iframe>

This visualization shows the sequences by open rate. Each sequence has been used to send at least 100 emails. The blue line that goes across the bars represents the average open rate across all sequences. Now we can clearly see which sequences outperformed the average as well as which sequences had the best open rate in descending order from best to worst.

## Insights

What stood out most to me most is that the majority of our sequences are at or above the 30% open rate threshold. The sequence with the highest open rate was the US - SDR - Marketing - SHRM Quiz - Hamid sequence at nearly 50%. The worst performing sequence was the US General 2 - Q419 sequence. With this information, I can analyze the possible characteristics of these sequences that made them work and also what made them fail. One contributing factor that would be interesting to analyze with my team is what types of subject lines did these emails have? Perhaps we will find a pattern there that can help us improve the sequences as a whole and avoid low open rates in the future. 

Another possible contributing factor to the vast difference in these two sequences' open rates might be the time of day that the emails are being sent. When someone receives an email is something that can greatly affect their engagement with it.

## Visual 2: Sequences by Reply Rate

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/14/#/" height="750" width="150%"></iframe>

This visualization shows the sequences by reply rate. Each sequence has been used to send at least 100 emails. The blue line that goes across the bars represents the average reply rate across all sequences. Now we can clearly see which sequences outperformed the average as well as which sequences had the best reply rate in descending order from best to worst.

## Insights

The first thing you might notice is that those beautiful colors from the previous graph are all scrambled. I did this on purpose to show how some of the sequences with higher open rates (the darker the bars the higher their open rate) are no longer the leaders when it comes to reply rate. Because different sequences have different messaging, this would suggest that the differences in the messaging within our emails matters.

Perhaps the most impactful insight that I gained from this analysis was just how effective the US SDR - Referral Sequence - Q120 is. With a reply rate of nearly 14%, it nearly doubles the reply rate of the next closest sequence and more than quadruples the average reply rate of just under 3%. This sequence includes both phone calls and emails, but what sets this sequence apart from the others is the fact that the people who are contacted through it are referred to us by people within their organization. To me, this shows just how effective asking for a reference can be and will definitely be something that I discuss with my team. 

## Visual 3: Open Rates vs. Reply Rates

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/78/#/" height="750" width="150%"></iframe>

This visualization shows the relationship between open rates and reply rates. Each sequence has been used to send at least 100 emails. The orange line that goes across the graph represents the general trend of the reply to open rate correlation: as open rates increase, reply rates tend to increase as well.

## Insights

The general trend is simple: the higher the open rate, the higher the reply rate. With that being said, there are two sequences that stand out. First, the US SDR Referral Sequence has a much higher reply rate than predicted. We can assume that this is mostly to do with the fact that we are working with referrals. The other sequence that stands out is the US - SDR Marketing - SHRM Quiz - Hamid. With an email open rate of 48%, its 3% reply rate is remarkably low. It seems like it would be worthwhile to either revamp the messaging of this sequence or stop using it altogether.

## Visual 4: The "True" Reply Rate

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/32/#/" height="750" width="150%"></iframe>

This visualization shows the relationship between open rates and reply rates through a metric I call the "true" reply rate. It shows how likely a prospect is to reply to an email given they have opened it. The blue line that goes across the graph represents the average true reply rate across all sequences. This is a feature that I engineered using the data from the total opens and replies for each sequence.

## Insights

The insights gained from this graph are similar to those gained from the previous scatter-plot: sequences that have a low true reply rate are sequences that could probably use some adjustments in their messaging while those with a high true reply rate can be used as models for other sequences.

## Thanks!

Well, that’s all I have for now. I appreciate you taking the time to read through this post! If you have any questions or just want to connect, feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/nathan-dow-42a846148/)!


