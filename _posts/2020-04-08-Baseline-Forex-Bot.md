---
layout: post
title: Baseline Forex Bot
subtitle: Random Buys and Sells
bigimg: /img/finance.jpg
---

## A Brief Introduction

One of my interests that pushed me toward data science is Forex trading. For more information about what the Forex market is, you can click [here](https://www.investopedia.com/articles/forex/11/why-trade-forex.asp).

To me, one of the most fascinating parts of the Forex market is the idea of algorithmic trading. In a nutshell, algorithmic trading is just waiting to enter a trade until certain conditions in the market are met. What makes it special though is that a computer is judging whether or not those conditions are met. In theory, if you have an algorithmic trading system that’s really good, you can consistently make money while you sleep! An exciting possibility if you ask me.

So, to get into this world of algorithmic trading, I’ve learned a lot about a trading platform called [Metatrader5](https://www.metatrader5.com/) and a programming language called [MQL5](https://www.mql5.com/), a language syntax that closely resembles C++. MQL5 is used to code trading ‘bots’, so to speak. 

Here is a sample of code that runs a simple bot that will enter buy and sell positions at random based on a randomly generated number:

```
#include<Trade\Trade.mqh>

CTrade trade;

input int TakeProfit = 100;
input int StopLoss = 100;
input int LotSizeFactor = 10000;

void OnTick()
  {
   //Calculate Lot Size
   double LotSize = AccountInfoDouble(ACCOUNT_EQUITY)/LotSizeFactor;
   LotSize = MathRound(LotSize);
    
   //Get a random integer to determine buy or sell   
   int random = MathRand();
   
   double Ask = NormalizeDouble(SymbolInfoDouble(_Symbol,SYMBOL_ASK),_Digits);
   double Bid = NormalizeDouble(SymbolInfoDouble(_Symbol,SYMBOL_BID),_Digits);
   double Spread = Ask-Bid;
 
   if ((random%2 == 1) && (PositionsTotal()<1) && (OrdersTotal() == 0))
      trade.Sell(LotSize,NULL,Bid,Bid + (StopLoss*_Point),Bid - (TakeProfit*_Point),NULL);
     
   if ((random%2 == 0) && (PositionsTotal()<1) && (OrdersTotal() == 0))
      trade.Buy(LotSize,NULL,Ask,Ask - (StopLoss*_Point),Ask + (TakeProfit*_Point),NULL);
  }

```
## In the future…

In the future, I will be posting more about algorithmic trading. I’ll be using this bot as the baseline bot to compare other bots’ performance. I will also be using this baseline bot to create sample data for future posts. 

Thanks for reading!
