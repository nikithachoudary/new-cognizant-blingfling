## Overview

BlingFling.com is an online marketplace aggregating the inventory of many jewelers around the world in one consolidated e-commerce destination.  This is a successful medium-sized business that is experiencing serious growing pains due to technical limitations.

The BlingFling website is powered by a crappy old PHP and MySQL site that was made from scratch by some barely-competent contractors who are now long-gone. An in-house engineering team was hired about a year ago, but they need help. 

Thus, Cognizant has been brought in to help recreate this rickety LAMP monolith into a modern microservices architecture. 

There is very little documentation of this system, but here are a couple of simple system diagrams showing the current situation.

<img src="https://i.imgur.com/ltYeoaA.png" height="400">

<img src="https://i.imgur.com/63Bq93H.png" height="400">

## Major problems the BlingFling team is experiencing

The site keeps falling over under load (e.g., during critical high-traffic times such as Black Friday weekend). The management team has responded so far by putting the site onto a bigger and bigger server. The network diagram shows that the site and database are now on a staggeringly huge EC2 instance.  This is very costly.

The BlingFling team is having a very difficult time adding important new features (such as free shipping), because of rampant regressions.  They have already largely reorganized their work processes around Agile/XP lines, but are having difficulty actually executing on their sprint (iteration) commitments due to the messy codebase. 

## Your task

Create a tech spec for BlingFling outlining the roadmap of migration from a monolithic system to a microservices architecture. 

Create documentation in Markdown format and use Draw.io (or Lucidchart, or any other tool that you prefer) to create system diagrams.

Apply what you have learned in the Cloud Native Developer course (and remember you can feel free to go back over your notes / look anything up -- it’s completely “open book”). 

* Which architectural principles and components do you recommend introducing?
    * Why? 
    * How do they address the problems above?
* Diagrammatically, what do these principles and components look like when assembled into the new architecture (say, a year or more from now)?
* What does a reasonable intermediate-milestone state of the architecture look like? (some months from now)?

Imagine that you are flying out to their corporate headquarters to give a presentation about your proposed architecture to seasoned engineers on their side.  They will be friendly, but as part of due diligence they necessarily will be probing your design for omissions and oversights. 

How do you prepare for this review session?  Anticipate a friendly-skeptical review -- what system design points are important to cover?  Make sure those points are adequately reflected! 

## Tips

* After you get the “happy path” sketched out cleanly, consider what would happen in various Bad Situations -- and how your design mitigates those problems.
* Think in terms of flows of processing through your components.
* Now what happens if a tidal wave of traffic were to cascade along those flows?  What fails, where, when, why? How to mitigate?
* Think about all the “-ity” concerns: scalability, reliability, security, maintainability, extensibility, etc etc.

## Q&A

#### How detailed should I get?
You have 90 minutes for this exercise, be as detailed as you can, but be sure to respond to all prompts.

#### Should this be a narrative or a bunch of diagrams?
It should be a mixture of both, use both types of artifacts as you see fit to get your point across.

#### How long should it be? How many diagrams?
That’s up to you, different people need more or less pictures/words to make their point.  Be sure you cover all the prompts though.

#### What type of diagrams are you looking for? 
This is up to you, but generally the straightforward “boxes-and-arrows” style of diagram is fine. (Much richer versions of the diagrams you see above in this document).

## How to submit your work

* Fork this repo.
* Commit your documentation artifacts -- diagram files / markdown files / etc.
* Push up your repo.
* Make a pull request back to the upstream repo.

