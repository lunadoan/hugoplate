---
title: "How to Design Success Metrics for a Feature Launch?"
meta_title: ""
description: "Measure success of a feature launch"
date: 2024-09-14T05:00:00Z
image: "assets/images/post1-define-success-metric.png"
categories: ["Measurement", "Product Development"]
author: "Luna Doan"
tags: ["metric definition", "feature launch"]
draft: false
---

How would you measure a launch success?

In this article, I'll borrow a question case from a Linkedin post.

**Question**: Our fitness app recently introduced a social feature, where you can add friends and share workout achievements. How would you measure the success of the feature? 

*(I change the question a bit, to focus more on metric definition rather than experiment design)*

My approach will be rooted on the data-driven case for decision making. Without further ado, let's dive in!

## 1. Start with a hypothesis
I always start off any analysis with a *hypothesis*. An user-centric plain English sentence of what the feature does to the users.

Assuming our fitness business has one goal: Make the world fit. And we've just built a social feature for our users.

My hypothesis then would be:

> The social feature makes our users motivated and come to us daily to stay fit.

{{< notice "tip" >}}
Writing hypothesis this way helps clear my mind before I jump into any outcome metrics, making sure I have a well-rounded measurement plan. The plain English also make it approachable to anyone.
{{< /notice >}}

## 2. Define success metrics
Recall the hypothesis:
The social feature makes our users motivated and come to us daily to stay fit.

With that in mind, I have 3 types of metrics to assess:
- Primary metrics: measure the outcome in the hypothesis
- Secondary metrics: measure the proxies of the outcome in the hypothesis
- Guardrail metrics / Countermetrics: measure the unintended user experience

### 2.1 Primary metrics
The primary metric I'd want to track is retention. As the frequency of workout ranges from daily to weekly for our user base (folks working out monthly would not be our customers), I'd like to track weekly retention: % of weekly active users come back the next week.

(Tracking weekly retention smooths out the noise, aka reduces the variance, which is better in most cases).

### 2.2 Secondary metrics
The secondary metric I'd want to track is **user engagement with the feature**. If users don't engage with the feature, yet I see an increase in weekly retention, **I'd suspect the result**. In data, *too good to be true is indeed too good to be true*. Tracking this type of metric make sure I spot the bugs which might be in the data tracking or the experiment setup.

For user engagement, I'd like to know:
- Number of sessions that the users use the social function
- Number of posts, messages, comments, reactions per user

I can go with number of sessions for simplicity, and go deeper and even break down to cohorts if I see a conflict among metrics or between the results and my hypothesis.

### 2.3 Guardrail metrics
Guardrail metrics, aka countermetrics, complete the picture of the feature impact. The whole purpose of these metrics is to make sure we don't create any unintended experience for our users. 

I'd like to evaluate:
- user engagement with other experience - do they watch training sessions less (and socialize more)?
- number of reports on inappropriate content/messages

I might want to track our customer service calls as well, as our users might feel confused or outraged about the new experience and need to call.

## Wrap up with a data-driven case
So, I have a measurement plan for the feature launch. After gathering the data and conducting the analysis, I now have a data-driven case for my business partners, helping them make an informed decision.

1) Do we see user retention move?
2) Is the movement aligned with other metrics, making it a reliable insight that we do see impact on retention?
3) Do we see any unintended impact, aka do we f*ck up?

> These insights will help my engineering and product team decide whether or not they want to roll out the feature / deprecate it to focus on other works.

Hope you enjoy this post! 

What would you approach this case? Let me know in the comment.

Feedback is most welcomed!

