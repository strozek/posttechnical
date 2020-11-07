---
title: "Just-in-Time Org"
date: 2020-08-24T21:27:42-08:00
draft: false
description: "A just-in-time approach to designing an organization."
tags: ["Organization"]
---
There is one systemic mistake that many leaders of young organizations tend to make: they _introduce structure that is premature_. This structure often looks like the much lamented "process", new restrictions or limitations, which generally hurt more than help, slowing down their teams' pace of development and agility. But this sometimes backfires in more sinister ways, actually affecting the outcomes, either because it discourages others from taking initiative, or forces a process that is suboptimal.

Examples of this mistake abound, and I dutifully report that I have made many such mistakes in the past. Some instances you may have witnessed yourself are:
* A performance management, promotion, hiring etc. process comprising dozens of steps, long forms, and taking weeks to complete
* Byzantine procurement or expense process that discourages people from creating leverage (or addressing problems) through spend
* Planning process where following the logistics takes more mental cycles than actually coming up with a plan
* Complicated code review and deployment processes that require a number of people to coordinate
* Restrictions on spontaneous self-structure activities such as creation of messaging channels or mailing groups
* Introduction of heavy-duty tooling and software that introduces more overhead
* Refactoring into a large number of microservices
* Consensus-based decision making, e.g. around engineering hiring
* An onerous process for proposing new features, which results in fewer people pitching their suggestions

The list goes on and on...

The leaders who make these mistakes usually have the best of intentions. So where do they go wrong? It is instructive to reflect on why these decisions are usually made in the first place.

The most common factor is that leaders are often _conditioned to build for scalability_. This is particularly true about leaders with a strong technical background – they have likely been burnt building software that failed to scale. But the issue with organizational structures is that, unlike with technologies, the downside of a premature structure is much higher than the (probability weighted) downside of a structure that no longer scales.

There are other drivers as well. Commonly, I see leaders who are scarred by their past experience and who want to proactively – and early – shape the operation of the team to avoid going down the same path[^1]. Maybe the Head of Engineering had a few bad hires in her previous company, is determined to lower the incidence of hiring "false positives" to zero, and created a "hiring by consensus" process that slows down hiring and lets in only the "safest" hires. Or a leader, who previously managed a team that pushed out a defective product, has vowed to never let that happen again and created a heavyweight deployment checklist which, again, slows everything down but doesn't actually protect against the bad outcomes the leader fears. The issue with overcorrecting for bad experiences is that when they happen to us, we tend not to maximize our learnings from them – certainly not in the moment. We don't run a quality post-mortem to gain an understanding of what the root cause of the problem was. Similarly, when faced with the new scenario, we don't reflect on the similarities and differences and we jump to a conclusion.

Another factor is a tendency to "let a single cut scar." More risk-averse leaders will _overly_ correct for bad outcomes, usually by adding more process instead of using the other levers that leaders have at their disposal (such as refactoring process or realigning people). The problem with such an approach is that it often masks the root cause (for example, an individual on the team who simply makes bad judgment calls, or a problematic aspect of the engineering culture that really ought to be corrected), and it erodes trust since the message the team receives is "the leadership doesn't not trust you to make the right decisions and is introducing process to safeguard against that."

There is also a perfectly rational explanation: leaders want to be helpful and add value. They are incentivized to "be leaders" – make decisions, be proactive about issues, _do things_. They will generally tend to act, even if they haven't fully formed a synthesis of the issue.

There are point solutions that can help mitigate each of the above scenarios. But I want to step back, look at the common theme behind them, and suggest an approach that structurally helps avoid many such scenarios.

> Issue: Fundamentally, issues arise when leaders and teams create new structure that isn't solving any problem, or that isn't solving _the_ problem.

I am a fan of lightweight structure because I have seen how it can transform teams and help them grow and continue meeting customer or product demands. However, this overcorreection is precisely what gives structure a bad reputation. An alternative approach I want to propose is the following:

> Solution: When making structural and process changes, decide as late as possible, that is, only when the existing structure is about to stop working.

It is a somewhat counter-intuitive approach. Often I hear teams say, "On no, we can't do this. It doesn't scale." But over the years I have seen that our technical intuitions fail us when it comes to structure. Organizational structures are usually more shallow than technical architectures, so long as the culture of the team welcomes organizational changes. This just-in-time approach also creates more organizational debt, but this is often a low price to pay if with it, we avoid possibly incurring very large amount of debt with one of these premature solutions[^2].

How might this approach be applied in practice? Let's take team structure, for example. Instead of structuring the team ahead of next year's roadmap, maintain the existing structure. It's likely that with it, we are effectively over-investing in some parts of the product and under-investing in others, so at some point lower priority features will be released faster than higher priority ones. When that happens (and only then), restructure the team to course correct for the priorities. It's possible that you'll only need to move a few people around instead of doing a full overhaul of the team structure.

Let's take another example from the list of mistakes above. Instead of introducing a complicated performance management process, reflect on what isn't currently working and address just that part. Do engineers complain that they don't have a sense of how they are doing? Ask managers to create that synthesis for them on top of whatever already exists for performance management, instead of instituting a whole performance review process. Do you think that not enough engineers are being promoted? Train your managers on spotting and growing highest performing individuals on their teams.

I'm not advocating that leaders shouldn't put in place large changes. But the magnitude of the change should be correlated to the magnitude of the problem, and to our confidence that we understand the problem and feel that the solution will actually address it. And most problems we encounter in organizations don't require large interventions.

I am, in effect, advocating for an incremental approach. As a result, changes will be more frequent, but their magnitude will likely be less. They will also be more "shallow," that is, easier to implement and easier to undo. There are some "good hygiene" prerequisites that can ensure that this approach works well. It's worth briefly discussing them.

1. Create a team culture of welcoming change, and a leadership competency of talking about change. Organizational and structural changes aren't something to be afraid of. Instead of saying, "_another reorg_," the team should welcome changes because – especially if they have faith that they address the emergent challenges – they help make the company better. Often this aversion to change is actually due to another leadership failure – lack of adequate communication and contextualization of the changes (changes happening in a black box), and a lack of perspective taking at the various layers of leadership to understand how each individual can be affected by the change.

2. Instil in the team, at all layers, a capability to form accurate _perceptions_ of problems, and do a thorough analysis of them and identification of _root causes_. While a more incremental and just-in-time approach to changes lowers the stakes involved in diagnosing the problems, it doesn't absolve leadership from the responsibility to know what problems they need to be solving.

3. Form a good set of intuitions about organizational debt. Is it so high that a large change may be needed? How would we know? Given the biases I've described above, the approach I would recommend we take is assume a large change is _not_ needed until proven otherwise.

**

A just-in-time approach to creating structure is not a silver bullet. But I encourage leaders to put it in their quiver alongside other techniques they've used before. At the very least, it is a good forcing merchanism for establishing better communication, an ability to diagnose problems, and a point of view about organizational debt on the team.

[^1]: The joke goes: to see what a leader disliked the most about their previous role one simply needs to find the largest solution to a nonexistent problem they introduced on the current team.
[^2]: This is analogous to the principle I described in [On Tech Debt](/posts/on-tech-debt) of intentionally managing tech debt, rather than just aiming to minimize it.