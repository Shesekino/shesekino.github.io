---
layout: post
title:  "Leading Without Authority: A Cautionary Tale"
date:   2022-02-06 14:00:00 +0300
categories: opinion leadership
published: true
---
Changing my role from an individual contributor to an architect, a role that relies heavily on one’s ability to lead without authority, had some challenges I did not expect.
The topic of leading without authority is discussed widely in books and articles, but I feel not enough emphasis is put on a couple of important related aspects.
This post will attempt to approach it from a different angle, observing the tension between authority and accountability, for technological leaders in software companies.

After a long career as a software engineer, I had a wonderful opportunity to move into a role as an architect. In a slow-paced, mature organisation, this role should be well defined and understood. In a young, rapidly growing and changing environment, however, a lot of even basic principles are vague or outright missed. A great deal of my energy had gone to trying to understand what this job, in this environment, requires of me.
I was “accountable, but not responsible”, for our product’s architecture: I needed to help the engineering teams in our group make the right strategic technological decisions, then see that we followed up on that.

To the best of my ability, and with plenty of help, I was able to come up with quarterly plans. After a round of reviews, a general agreement among the group was reached, and on the surface it looked like I'd been able to satisfy my requirements.
And then… reality kicked in. Sprint after sprint, I realised our group is consistently choosing new feature work over the plans we agreed to. It was clear something wasn’t working well, but it was hard to point out exactly what or why.

During the months that followed I would reflect on my role and on the sustainability of our current situation in the long term.

## Authority and Accountability Relationship

> In the context of this post, **Authority**, direct or borrowed, is one’s right to give orders and make decisions, on behalf of their organisation.
**Accountability** is one’s ability to be held accountable for these tasks’ executions and impact: Have they contributed to the organisation and the product as they should have? Was the investment worthwhile? Did we make the right calls?

*In a state of equilibrium, the relationship between Authority and Accountability has to be linear and aligned.*

What I mean by that, is that if and only if someone is accountable for getting something done, they’d need the proper authority (direct, or borrowed) in order to efficiently make it happen. To justify that claim, let’s examine four different configurations of authority and accountability.

### High authority, high accountability: Partner

In this state, you’re expected to lead (a project, a task) alongside an engineering team, with sufficient authority and accountability. It’s pretty straightforward in the sense that everything, for better and worse, is on you: You call the shots, you make the final decisions, and if something goes wrong, you should be able to explain why that happened and how you’re going to handle that. That makes you fully invested in making the project successful, and a full partner through it all.

Overall, this state is sustainable because the toolset you’re given is sufficient to get the job done. If the project fails, there’s a good chance you made some bad decisions along the way, and there’s things you can improve for next time.

### Low authority, low accountability: Consultant

In this state, an engineering team needs to deliver a project, and you’re asked to assist. Your experience and broad view of the organisation gives you a valuable perspective which can benefit the team’s execution, and you can and should provide as much guidance as necessary to make the project successful - but at the end of the day, you don’t own the delivery of the project. You’re not the one making the final decisions, and that’s okay, because success (or failure) won’t be attributed to you.

This state is sustainable because even though you’re “just” providing counsel, you’re also not held accountable for things not under your control.

### High authority, low accountability: Gatekeeper

In this state, an engineering team needs to deliver a project independently, and you’re asked to assist. You also get to say the last word on the tech decisions, but neither the success nor the failure of the project will reflect on you.
The problem in this scenario is that even though you’re not invested in the success of the project, you still act as a gatekeeper for major decisions. You’re more likely to be interested in things getting done “the right way technologically” over the right way for the organisation which probably includes some concessions. Moreover, you have very little incentive in actually facilitating that happening.

At some point, people would start noticing you’ve become a bottleneck and that you generate more noise than actual help, and you’ll become obsolete. That’s why this state is not sustainable.

### Low authority, high accountability: Diplomat

In this state, you’re expected to lead (a project or a task) alongside an engineering team. You have some influence, but don’t decide the team’s priorities.
When your goal and the team’s goals are fully aligned, there’s mostly no friction and we can expect this to work pretty well. In reality, an engineering team has many incentives and external, immediate pressure from stakeholders - many of them would have nothing to do with your goals. It is inevitable that a lot of these cases would result in high friction situations where someone needs to decide between immediate and long-term strategic goals. With only some influence, you can invest a lot of time persuading the team to align with your goals, but this is usually an uphill battle, since long-term investments are harder to understand and prioritise when more tangible tasks are present.

An imaginary example could be having to choose between implementing a large, complex feature a specific customer requested, that would significantly increase the team’s technical debt, or investing the same amount of effort in restructuring the team’s infrastructure, significantly reducing “cost of change” for the next ten features or more. When faced with a concrete customer need, an engineering team is more likely to choose working on that over a long term investment in their sustainability.

This means that in order for you to have any significant impact on the team's plans, you'll need to invest hours negotiating with multiple different stakeholders for even the smallest pieces of work to get done. It's not impossible, but it's probably not worth it.

This state is unsustainable because the set of tools you’ve been given is insufficient to get the job done in a reliable manner - you’re unable to commit to any kind of timelines, and even getting small things done requires a lot of inefficient, hard work of convincing and diplomacy. It’s exhausting, frustrating and provides little value  in the long run. In this situation it’s more likely you’ll get better results by either dropping the project or working on it alone. In the long run, you’ll recognise this kind of situation before getting into them in the first place, and avoid them.

## Takeaways

Since then, whenever I approach a task that relies heavily on *leading without authority*, I’m more careful to set expectations early on around:
* What exactly is everyone involved accountable for
* What kind of authority, if any, do I have
* What kind of conflicts might the different parties involved have and how would we go about resolving them as a group

If I have no authority over the work, I can still be a valuable consultant to the team. High authority and accountability means I’m a full partner through thick and thin. Any other way is unlikely to result in success.

Here's a simple matrix to print and hang on your wall for reference:
![authority-accountability-matrix](/assets/authority-accountability-1.png)
