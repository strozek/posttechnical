---
title: "On Tech Debt"
date: 2020-10-01T21:57:01-07:00
draft: false
description: "We interact with tech debt so much in our engineering lives, yet we rarely reflect on it. How should we think about it? How should we communicate it to others? What are our blind spots around it?"
tags: ["Software Development"]
---
So much has been said about tech debt that it almost feels trite to cover it. Our stakeholders nod understandingly when we mention it; the Product folks considerately ask if we want to work on tech debt in the upcoming sprint; our own team attributes their missed deadlines to tech debt... it feels like an omnipresent phenomenon that we all know what to do with. Yet when asked to explain tech debt, stakeholders draw a blank; PMs say it's an internal tech thing; and our team may be hiding behind a convenient excuse. Perhaps it's time to dig a little deeper into tech debt.

Technical debt is a metaphor first coined in 1992 – which seems like another era when you think about software development. [Martin Fowler](https://martinfowler.com/bliki/TechnicalDebt.html) has a nice explanation including the origin story. To spare you a click: over time (and under a variety of other circumstances), code degrades in clarity, which introduces a cost to future velocity of development and stability/robustness of the system. This degradation is likened to the "principal" of a financial debt, and the resulting costs are the "interest". If you don't improve the quality of the code ("pay down the principal"), you will have to pay the costs over time, often many times over the cost of the actual improvement.

Here are a few possibly nontrivial observations on tech debt.

## I.

First, the reason why I really like the comparison to financial debt is that the analogy holds in one crucial, but counterintuitive, aspect.

In a healthy economy and with healthy household finances, _some amount of responsible financial debt is rationally optimal_. Take me, for example. I am still paying off my student loans but the interest on these is a little less than 2%, which is half the interest I could make on my money in minimal-risk digital asset credit markets (let alone the 13.6% annual return one might have enjoyed on the stock market over the last 10 years). I also take out debt in order to take advantage of money today (buy a house) while spreading the cost over the next 30 years. Similarly, in a company with a healthy product development process, some amount of tech debt is also optimal, and there are circumstances where we may explicitly want to take on technical debt – akin to a mortgage.

I suggest we stop only caring about debt when there's too much of it, or – conversely – as something to be reduced to zero, but as something to be managed depending on our circumstances. For example, if the opportunity cost of taking even a few days more to build a new feature is high, it's reasonable to take on a large amount of technical debt just like one would take out a mortgage, but then it's important to set aside ongoing bandwidth to pay down the debt, just like one would ensure they have enough income for the the monthly mortgage payments.

When might be make sense to _refinance_ the technical debt, i.e. change our approach and pay the debt off differently, over a longer time period but with less daily overhead? What could that look like?

## II.

Engineering teams always, _always_, underestimate the effort involved, and overestimate the benefit of addressing tech debt. Much has been written about it but in brief, because engineers are able to envision the end state easily, this gives them the impression that they are closer to the end state than they actually are. As for the benefit, unlike in financial debt, we can never fully pay down the principal – **any code we write embeds assumptions about the world**. Unless we can perfectly predict all future use cases, our code will not be optimally structured for _all_ future work.

One could add "fudge factors" to address this bias but I don't recommend it. Buffers are a good technique for expectation setting, but they detract us from understanding our practices better. Instead, the best mitigation is also the most boring (and hardest to implement) one: make all improvements to the codebase _gradual_ so that you can get better at projecting both the cost and the benefit better. Of course, incremental approaches aren't possible for every refactoring, but even when they are, teams too quickly give up, seeing an incremental approach as inefficient.

If they can suspend their disbelief and embrace an incremental approach, teams may soon discover that by _designing for this incremental approach_ they can manage tech debt better. For example, instead of trying to over-optimize their code upfront, teams could focus on discovery and iteration first, even if it makes them repeat themselves or use a more "flexible" design pattern instead of one that is more "appropriate", but less forgiving. Yes, this will create more tech debt upfront, but the payoff will be shorter.

## III.

Business stakeholders _think_ they understand tech debt, but for someone who is not technical, the analogy to financial debt may not be that helpful since they may find it hard to map the insights and consequences that may be clear in the financial domain to the technical one. Most stakeholders I've worked with understand that there are some hidden costs of moving fast, or of old code, but it's difficult for them to reason beyond that. Similarly, while some more technical product managers may have a good intuition about tech debt, usually PMs leave it to tech leads to manage tech debt in ways that best serves the team, thinking of it as an item internal to the engineering team.

I would argue that _of course_ the PM needs to care about and understand the nature of tech debt. _Of course_ the stakeholders need to care about tech debt. Tech debt is not some "implementation detail" that affects just the engineering team. It's an important input into the most important question that capable tech leads can answer for PMs and stakeholders – namely, "How long will this take, what are my options, and what are the trade-offs?"

Perhaps a more useful way to think of tech debt in this context is to start by considering the time horizon of technical investments. If teams adopt a short time horizon when calculating ROI, most work ends up getting done reactively to address the most pressing problem facing the company, to chase the largest deal, etc. (Sales-driven cultures often use a short time horizon). Effectively, the discounting factor is very high – it isn't that useful to deliver something in a year – and companies end up with high tech debt and expensive technology development because investments in tech debt just don't bring a high enough ROI. On the other hand, companies that think long-term – maybe strong vision-driven cultures – calculate their ROI over an extended period of time and for them, it absolutely makes sense to lower the amount of tech debt. Their discounting factor is low – they are playing the long game.

Often, Engineering, Product and the business stakeholders do not agree on what discounting factor to use, which could cause misalignment on tech building decisions. The critical corollary is that business stakeholders or PMs absolutely need to understand these trade-offs, and thus tech debt. It should never be something that the engineering lead is trying to "squeeze in" or that the PM is setting aside as the engineering lead's discretionary "budget".

**

Technical debt isn't as well-known a quantity as some may seem to believe; teams have misconceptions about it that may be slowing them down. A good way to engage with tech debt, in my view, is to identify the "healthy" amount of target tech debt to take on depending on business circumstances and be disciplined about paying it down, also at a "healthy" pace. When paying the debt down, teams should try to find incremental approaches to lower the "total finance charge". Finally, engineering teams should make it a point to ensure that the stakeholders and product owners understand tech debt and the implicit trade-offs well. The best way to explain it is by aligning on the "discounting factor" and then reframing tech debt as a driver of trade-offs between short-term and long-term impact.
