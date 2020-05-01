---
layout: post
title: Food Waste Data Exploration Part 1
subtitle: Sample Dataset 
bigimg: /img/veggies.jpeg
---

## What: 

This project is one that focuses on my idea to use data in order to incentivize businesses to reduce the amount of food they waste by tracking that food and redistributing it to those who could use it. 

This post dives into a sample dataset of my own creation that shows some potential data features that could be collected through this process as well as some features that could potentially be engineered and the visualizations that businesses could use to understand what food they’re wasting and how much it’s costing them.

## Why:

There is enough food for everyone but not everyone has enough food. According to the USDA, [37 million people](https://www.feedingamerica.org/hunger-in-america) struggle with hunger in the United States, yet in 2017 we disposed of [38.1 million tons of food](https://www.epa.gov/recycle/reducing-wasted-food-home). Figuring out how to capture and redistribute some of this wasted food seems like a problem worth solving.

## How:

The idea is to have businesses work with individuals who are food insecure. These individuals would go to the business, weigh the would-be wasted food at the end of the day, input a few simple data points in a spreadsheet, and in turn, be able to use the food for themselves at no charge.

The data entry that the individual would oversee might include the following:
- The date
- The day of the week
- The type of food
- The quantity of food leftover
- The location of the business
- The employee

After converting the spreadsheet into a CSV file, we would turn it into a data frame that looks something like this:

![Sample Table](https://raw.githubusercontent.com/ndow33/ndow33.github.io/master/img/table1.PNG)

Once in this form, we can collaborate with the business to engineer features that would provide valuable insights such as:

### Leftover food by month

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/123/#/" height="750" width="150%"></iframe>

### Leftover food by day

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/117/#/" height="750" width="150%"></iframe>

### Total leftover food

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/120/#/" height="750" width="150%"></iframe>

### Lost revenue by month

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/132/#/" height="750" width="150%"></iframe>

### Lost revenue by day

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/126/#/" height="750" width="150%"></iframe>

### Total lost revenue

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plot.ly/~ndow33/130/#/" height="750" width="150%"></iframe>



While these graphs are simple rough drafts, these insights, along with others, could help businesses understand how much they’re wasting in order to help them reduce their waste. Until that waste is reduced, they can feel good knowing that the people collecting the data are in need of the food they would otherwise be throwing out.
