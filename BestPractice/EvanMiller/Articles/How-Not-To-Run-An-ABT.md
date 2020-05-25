# [How Not To Run An A/B Test](https://www.evanmiller.org/how-not-to-run-an-ab-test.html)

> By Evan Miller (April 18, 2010)

If you run A/B tests on your website and regularly check ongoing experiments for significant results,
如果你正在你的网站上运行A/B实验，同时对于正在运行的实验定期检查重要的结果，
you might be falling prey to what statisticians call repeated significance testing errors.   
你很有可能碰到统计学家所说的“重复显著性检验错误”。
As a result, even though your dashboard says a result is statistically significant,   
there’s a good chance that it’s actually insignificant.   
因此，即使你的统计面板显示结果在统计上是显著的，也很有可能实际上是不显著的。 
This note explains why.  
这篇文章会解释为什么。

## Background  

背景

When an A/B testing dashboard says there is a “95% chance of beating original” or “90% probability of statistical significance,” it’s asking the following question: Assuming there is no underlying difference between A and B, how often will we see a difference like we do in the data just by chance? The answer to that question is called the significance level, and “statistically significant results” mean that the significance level is low, e.g. 5% or 1%. Dashboards usually take the complement of this (e.g. 95% or 99%) and report it as a “chance of beating the original” or something like that.

However, the significance calculation makes a critical assumption that you have probably violated without even realizing it: that the sample size was fixed in advance. If instead of deciding ahead of time, “this experiment will collect exactly 1,000 observations,” you say, “we’ll run it until we see a significant difference,” all the reported significance levels become meaningless. This result is completely counterintuitive and all the A/B testing packages out there ignore it, but I’ll try to explain the source of the problem with a simple example.

## Example  




