---
layout: post
title:  "The Task Force Fallacy"
date:   2022-03-26 10:00:00 +0300
tags: opinion project
published: true
---

Once in a while, an unusual task presents itself to an organisation. A framework needs to be replaced; A monolith needs to be broken apart; Infrastructure changes require some coordinated effort. Whatever the task is, it doesn't fall cleanly into a specific team's domain. Moreover, there's an expectation that it's a one-off - a concentrated effort for a short period of time (weeks or few months) will put a big enough dent in the task, and the organisation will be back to business as usual.

This scenario often calls for a *task force* (or multiple *task forces*) - a team-sized (or less) collection of engineers from different teams, sometimes from different parts of the engineering department, banding together for a specific cause for a limited amount of time.

In this post I will present the attractions of such task forces and why I believe it's an organisational anti-pattern you should avoid, unless you absolutely know what you're doing.

* TOC
{:toc}

## The Appeal

![task-force-example](/assets/task-force-fallacy-1.png)  
*A classic task force, comprised of four members from four different teams.*

### Easy to Understand

Task forces are similar to teams in many aspects, making them easy for an organisation to understand. They are composed of multiple engineers, assigned a lead, communicate through whatever means the organisation uses to communicate, etc.  
With a broad task to be done, it's easier to assign a single unit of people as responsible, and their lead as accountable for execution of the task, as opposed to slicing responsibilities across multiple teams. If a manager needs to know how the project is doing, they only need to ask one person for the account, simplifying project management.

### Short Communication Paths

Short communication paths are vital for any successful collaboration. If I'm sitting in the same (physical or virtual) room with the people I need to work with daily, I'm more likely to communicate effectively.  
For tasks that require a broad spectrum of expertise and members of the organisation, the act of unifing them as a task force helps shorten their communication paths. Moreover, temporarily removing someone from their usual team might help them consider the solution with a more objective perspective that's less influenced by their place in the organisation, avoiding sometimes undesirable effects of [Conway's law](https://en.wikipedia.org/wiki/Conway%27s_law).

## The Catch

And yet, every time I see someone proposing setting up a task force, I get a little uncomfortable, and for good reasons.

### Timelines, Deadlines & Definition of Done

One of the few things I remember from studying mechanics in high school is that `distance = speed * time`. In software engineering, the formula can roughly be represented as such:

`distance`: The size of the task that needs to get done, represented by a concrete "definition of done" (e.g. "Migrate the CI/CD infrastructure for all the production services."). While the definition of done is clear and common for everyone, the steps required to accomplish it may vary for different components in the system.

`speed`: How many engineers, in what capacity and with what level of seniority are involved. Speed is capped at some point, because having too many people working on a task will just slow it down.

`time`: How long will the task force exist.

Unlike most high school problems I had to solve, in software engineering the distance is incredibly difficult to measure, especially for bigger tasks. This uncertainty would manifest in the task force in at least one of the following ways:

`distance`: The task force will not accomplish its designated goals on time.

`speed`: Some engineers may drop off during the work, as their managers will apply pressure to get their team members back.

`time`: The task force will continue working past the estimated timeline.

Projects and tasks getting dragged or delayed is not a new thing - but if it happens in a foreign construct (task force) then handling these delays becomes more difficult.

### Ownership & Handoff

Software in an organisation is usually owned by teams. In order to modify software, the owning team members need to either introduce the changes themselves, or thoroughly review external requests.

On the surface, the task force respects this model by including a team member from teams with software relevant for the task. Changes to that team's software will go through their team member who would take care of spreading knowledge and responsibility in their original team for long term ownership.

In practice, members of the task force are incentivised to progress primarily on the task force's immediate goals, and not on empowering their team to own the new software. Ironically, the team is entrusting their "loaned" member to represent the team's long term interests, and prefer putting the changes out of their minds until the task force finishes its work - that's why it was created in the first place, right?

When the task force does end, the team will continue their business as usual with their long gone member back. The task is (hopefully) done, and a new sprint with new features can begin. But what's going to happen with the knowledge gap around the new software that the team now supposedly owns?

### Leadership

Teams are managed by engineering managers (team leads): Experienced people hired or trained for the complex role of managing engineers and being accountable for projects they oversee. When forming a task force, organisations will usually look for someone to be accountable for the task, but it's difficult to find someone - all the team leads are taken!

To compensate, one of engineers on the task force will be asked to lead it: coordinate the different members, communicate with stakeholders, make sure progress makes sense with regards to the timelines, etc. This is often portrayed as a high profile growth opportunity for an individual less experienced with leadership - and it is - but it also means that the task which was so important for the organisation to push, and so complicated it needed a task force, is being lead by someone sometimes insufficiently experienced to lead it successfully.  
Additionally, if the task force's lead also happens to be an experienced engineer with the most context for solving the task, then their time would probably be better spent in a more technical role.

## Then What?

Okay, task forces are difficult to run, but the kind of tasks that call for task forces will continue to exist. How can we handle them better?

### Practice

Some of the difficulties I mentioned on running task forces can be mitigated through intentional and repeated practice. If an organisation has frequent needs for task forces (which should probably raise a red flag by itself), then explicitly stating a goal of improving how they run task forces can be useful. Invest in how task forces are created, define and communicate their goals, help teams own changes to their software and improve individuals' leadership skills through deliberate exercises and training, and over time you'll become better at running task forces.  
That's a lot of investment for something considered out of the ordinary though.

### Project Management

Teams exist for a reason. Instead of going around their purpose, harness it. This means that instead of having a task force with four members, one from each team, you'll need to break down the task to smaller pieces of work and coordinate it with the four different teams. This means more project management (and potentially assigning a project manager to coordinate the work), but it also means that all the disadvantages that arise from bypassing the organisation's basic unit of delivery - teams - should be gone.

### Study Groups

There's a concept I'm experimenting with around *study groups*. Study groups are structured similarly to task forces, but completely differ in their purpose.

I plan to dedicate a post for the study group, but these would be the key differences:
* While a task force delivers software, a study group gathers knowledge and delivers it to their teams.
* A task force may exist for months, but a study group can be timeboxed to one or two weeks.
* A task force requires a central lead, but a study group can function in a distributed way more efficiently, each person being accountable for their own learning and growth.

## Closing Thoughts

Solving a wide problem that can't reasonably be handled by a single team is difficult, however you look at it. There's different ways of doing that, each with its ups and downs. I believe the simplest way - forming a temporary task force - is also inferior in many ways and should be avoided, unless your organisation is well practiced in it. Favouring knowledge gaining and sharing over short term software deliveries will have long term benefits and long lasting positive effects on teams.
