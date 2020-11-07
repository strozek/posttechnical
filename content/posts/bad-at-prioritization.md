---
title: "We're All Bad at Prioritization"
date: 2020-11-03T23:08:47-08:00
draft: false
description: "Let's face it. We are all bad at prioritization. Let's identify some traps we commonly fall in so that we can create forcing mechanisms around us."
tags: ["Product Management"]
---
Prioritization is one of the few foundational capabilities. We all need to do it: whether we are a junior engineer or a CEO; at a macro level (what should the team work on in the next quarter) and a micro level (which emails do I respond to today); whether we're in Product, Engineering, or any other function in the company. We do it very explicitly ("Product Roadmap Prioritization Exercise"), somewhat explicitly (pick an issue out of the backlog), or implicitly (going through the Slack messages in the morning).

And there is one thing that is absolutely true about prioritization: we are all relatively bad at it. Worse, we don't even stop to think about _how_ bad we are at it. We don't look back to see which emails we responded to and which we didn't. We don't run post-mortems around the roadmap items we did _not_ pick up in the quarter. A common excuse to something important not being done is "I didn't get to it" or "I had way too much on my plate." And while the ability to prioritize well is critical for some roles (e.g. Product) and seniorities (e.g. CEO), I believe that it's a skill that, when perfected, will make everyone significantly more effective and propel them in their career.

## What does it mean to prioritize?

This may seem like a strange question. Prioritization feels like such an obvious activity: figure out what's more important and do it first. But there are actually a number of nuances involved in prioritization:
* What time horizon are we looking at? Are we prioritizing things that have an ROI that's realizable within a day, or two years? How to compare these two? And, assuming that we can, how do we prioritize items which will take a long time to complete?
* Who defines what is "important"?
* Who should do the work?
* What are we _implicitly_ prioritizing by not questioning them, or by not doing other things instead (opportunity cost)?

If we reflect on these questions, it may become clear that prioritization often seems that it is not well-defined. We are asked to compare apples to oranges, and make decisions that collapse the opinions of multiple parties. We have to run all sorts of counterfactuals and think of a "white space" that is practically infinite. It's easy to be discouraged.

The best advice I can give is to be pragmatic. _Of course_ we won't be able to come up with a perfectly optimized prioritization process that captures and quantifies all the aspects of importance. But with some discipline we can capture 80% of the value. The above considerations are helpful, though, in identifying possible blind spots – items that easily fall in the 80% but ones we just forget to think about.

And speaking of blind spots, before we cover some techniques, it is helpful to understand what the common failure modes are.

## How do attempts at prioritization commonly fail?

### 1. The What

The single largest factor that contributes to poor prioritization is the lack of guiding principles, a north star, or a clear and comprehensive vision that we should prioritize our work _against_. If we find ourselves reinventing the wheel with each prioritization decision, making one-off decisions that don't seem consistent over time or generally feel unsure of the answers, we probably haven't done enough prep work. In an ideal world, prioritization is easy because we've already defined the ground rules for our decision-making process, and all we need to do is apply them. Realistically though, vision, a north star, a strategic direction, or however we think of the future state, is hard to establish, and there is often a feedback loop between the decisions we make and the vision we're driving towards.

Some biases that are often at play during prioritization are the _recency bias_ (overindexing on things that have happened more recently), _availability bias_ (focusing on things that we can recall better or that are more top of mind) and "completeness bias" (my term which I'm sure has an official version), which is a common phenomenon of focusing on what is more completely defined – for example, a more comprehensive product spec – instead of what is more important to do (but maybe harder to define).

### 2. The Who

In the absence of a clear set of guiding principles, teams experience what is commonly referred to as the "squeaky wheel" problem. Priorities are often hijacked by inputs unrelated to the importance or urgency – often something as simple as how vocal (or annoying, or nagging) the requestor is. A version of the squeaky wheel problem is being overly reactive to what competitors are doing. Or one group simply creates a lot more requests than the others and thus starves out the other work. Similarly, we often don't prioritize invisible things highly enough, especially _unmanifested risks_ and _foundational issues_. This can be seen often when teams complain that the company puts too many resources in the product work at the expense of the infrastructure or platform work. Other faults include misclassifying opinions as facts, prioritizing work just because someone feels about it strongly, rather than because there is evidence that it should be prioritized.

### 3. The When

Another factor is a difficulty in reasoning through different time horizons, and executing in ways that are consistent with the answers we came up with. At the simplest level, this manifests as the "important vs urgent" dichotomy: we struggle when mixing together work that has a short deadline, and work that may have a higher total return on investment, but that can wait to be completed. Even if we can come up with some allocation of resources (e.g. spend 50% of your time on the urgent, and 50% on the important), the former takes up more time and the latter always gets pushed out.

### 4. The How

There are a number of ways to implement a prioritization scheme. One more recent way that has gained in popularity is **business value voting**: a protocol where stakeholders get a number of votes (key ones get more votes) and they get to vote on roadmap items that they would like to see implemented. I personally believe that such a system is a terrible idea. It is precisely the type of scheme that gives everyone the _impression_ that they are coming up with the right priorities. There are multiple issues with business value voting:
* Stakeholders fall prey to the same biases I described above. Having all stakeholders in the room vote together doesn't eliminate the biases because they are highly correlated with each other; it magnifies them
* A "vote" is a very low fidelity method of signaling a very complex set of preferences. A single vote is supposed to unify the concepts of time horizon, dependencies, technical risk, incremental milestones, and the difference between effort and duration
* The voting process is highly susceptible to how the items are presented and promoted in the room. I don't mind making a good pitch be a prerequisite of investing in work, but the business value voting is a highly condensed, high stakes, one-time event that magnifies the effect of pitching on the end result

There is a (good, in my view) reason that our everyday politics is, theoretically, a representative democracy. We don't vote on all issues; we elect people who represent us and vote on issues for us. In organization, such a group is the Product team. And while the PMs don't vote (another reason to be skeptical of business value voting), they have high-context, rich debates about what to work on when, bringing in experts when needed, and checking in with stakeholders, carefully balancing the complex needs. That's their job and they spend years perfecting their craft.

## How to develop the muscle

It helps to know what _not_ to do. But there are also constructive ways to get better at prioritization. I believe it's to a large extent a muscle: there are some key prerequisites such as attention to detail, ability to reason and diagnose issues, but practice is the largest driver of success. That said, below are some techniques that may be helpful when going through prioritizing exercises.
* Identify areas that feel most like "apples" and "oranges." These are the areas where ongoing prioritization will be the most painful, and may just not be possible. Instead, define _a priori_ some division of resources and cut through prioritization that way. This is often done with items which are foundational in nature – companies set up separate teams, or some specific amount of team bandwidth on these. For individuals, this could look like specific days or time blocks set aside on the work which wouldn't otherwise get its fair share of time.
* To deal with the "squeaky wheel" problem, pass all requests though the same "band filter". Extract the substance but leave behind the emotion. If you have a wide variance in the frequency of requests (or loudness of "squeaking"), use the above technique to load balance the requests
* For items which have varying time horizons, come up with an appropriate "discounting factor" for time that depends on the stage the company is in, or the importance of time to market. If you imagine the prioritization being an ordering of weights of the different items, the discounting factor is a multiplier to the weight (that is less than 1.0), which gets applied if the work doesn't have to be completed until some time in the future.
* For any items for which there are prioritization headwinds (e.g. tech debt which has a future-looking benefit, often in the form of preventing future risk), see if you can convert them to the more "vanilla" items. Is there a milestone that provides incremental value? Can you quantify the risk as (_probability_) * (_cost if the risk happens_)?
* Call out possible biases that you or others who provide inputs into prioritization have. Can you try to identify where bias has had an impact, and explicitly course correct? For some items, you may be able to ask yourself, "What would I want to figure out, of what would have to be true, for this item to be prioritized more highly?"
* QC the resulting priority queue. Pick two items at random, not too far from each other, and ask yourself: are they correctly sorted given everything I know about them? Sample a number of times to make sure the priority queue is solid
* To address the completeness bias, require that all ideas have a basic level of definition, but explicitly ask for a limited amount of detail. If an item can't be described in a few paragraphs, is it really important?
* Create more transparency around the intermediate work items, and the final roadmap. The downside is you having to explain yourself more, but the benefits are worth it
* See if you can catch yourself making implicit prioritization decisions. For example, at the end of the day reflect on how you spent your time and what decisions you made to reach this distribution. What else could you have done? Why didn't you? Was this the right call (with the benefit of hindsight, and without it)?

These are just some techniques to apply in our everyday struggles with prioritization. Even though many examples I gave have to do with product work (feature prioritization etc.), the skill applies just as much to engineers – if not more. After all, between picking up work, deciding what parts of the codebase to improve, and making hundreds of little decisions, there is quite a lot of prioritization to be done, much of it hidden from sight.
