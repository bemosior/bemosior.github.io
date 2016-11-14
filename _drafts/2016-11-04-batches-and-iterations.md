---
title: Batches and Iterations
image: 
date: 2016-11-04
---

TK Get rid of "batches"

The goal of software development is to deliver value to the customer in the form of working software. To accomplish this feat, there may be various stations of work (product, development, quality, operation, etc.) involved, each composed of people. Let’s call the whole thing “software-building.” “Batches” are the units of work into which “software-building” is broken down for purposes of completion during an "iteration," the cycle that begins with an idea and ends in working software. A "feature" may be composed of several units of work.

“Smaller batches” just means greater granularity compared to what you are doing now. If you deliver all the software in one batch, consider breaking the work into more batches. If you deliver one feature per batch, consider breaking the bigger features down so they can be delivered in multiple, smaller batches. Push the limits of what seems reasonable until you know you’ve gone too far, then pull back just a bit.

Ok, but why make batches smaller at all?

* Uninterrupted time is precious and rare for many. Less work to do per batch means less context to build and rebuild every time someone sits down to do the work.
* The problems are smaller, meaning they are easier to tackle, describe, and get help with.
* Smaller batches are finished faster, enabling greater flexibility for how people can use their time.
* Smaller batches enable shorter iterations.

---

For most software-building systems, there is a concept of “iteration,” which may be expressed as a number, rate, or continuity. As a number, it may be “zero” (if the software is never delivered), “one” (if the software is delivered all at once), or “y” (if software is delivered multiple times). As a rate, it may be “y per z” (deliveries per time period). As a continuity, every change may be immediately delivered (i.e., “continuous delivery”). In all cases, the software delivered encompasses some number of completed batches of work. Let’s focus on iteration as a simplistic “1 delivery per time period,” since that is where many begin. Like batch sizes, start where you are and consider reducing iteration length until it’s as short as it can be (it will need to be equal to or greater than the smallest batch size). As the iterations grow shorter, it’s important to recognize the pain points of the process and fix what hurts.

Ok, but why make iterations shorter?

* There will be more opportunities to scope, perform, reflect, and adjust work, meaning a greater chance of accommodating change and building the right thing.
* Shorter iterations counteract Parkinson’s Law, which states, “work expands so as to fill the time available for its completion.” A near deadline enables focus and encourages work to be finished earlier. (To be clear, it’s not a stick to beat people with. If the batches are small, the nearness of the deadline will not be difficult.)
* If the work is “all wrapped up” on a more frequent basis, that means more opportunities to cleanly release and ship the software to the customer. It’s still a business decision whether to do so, but the software-building process will constrain the business less.
* Shorter iterations reinforce the need for smaller batches, creating an enabling cycle.

Shorter iterations, if coupled with smaller batches of work, enable greater “flow” of work through the software-building system, enabling more of it to get done.

---

This post may, to some, be about Agile. If so, please read [The Agile Manifesto](http://agilemanifesto.org/) and accompanying [principles](http://agilemanifesto.org/principles.html). Read them both at least three times so they are fresh in your mind. Do it now; it won’t take long.

As you have just (re)discovered, Agile is based on values and principles, with which you may or may not be completely aligned. Value systems are not transplantable, however, so recognize that you can only start from where you are and move in a new direction.

Understand also that Agile is a context-dependent methodology, best suited to particular kinds of circumstances (not one-size-fits-all). Dealing with uncertainty is its bread and butter. For many software development projects in the early stages, uncertainty abounds, and Agile is a strong pick. Again, a value system cannot be transplanted, so there isn’t much “picking” occurring in the first place, but we’re going to hand-wave that for now, as you don’t need Agile to leverage batch and iteration size to get more software-building done.