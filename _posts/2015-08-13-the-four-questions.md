---
title: The Four Questions
image: 
date: 2015-08-13
---

Dr. Eliyahu M. Goldratt, in his lecture titled [Beyond the Goal: Theory of Constraints](http://www.amazon.com/Beyond-Goal-Theory-Constraints/dp/B000ELJ9NO), describes the necessity of answering the following questions when adopting a technology:

1. What is the power of the technology?
2. What limitation does it diminish?
3. What rules helped us accommodate the limitation?
4. What rules should we use now?

As a cofounder of a small software development business, I thought it would be interesting to describe how we applied this approach to a technology-oriented decision.

<hr>

Several months ago, we developed a business process application for one of our clients, making use of Node.js and a relatively new framework (stop laughing). As the market shifted, so did the client’s business needs and goals, and we built out new features or adjusted previous ones to accommodate. However, we began to feel that our design and development process, as it pertained to the technologies we were using, had become a severe limitation. As we started planning the next major version of the application, we decided to make some changes. One of our cofounders had been looking into Laravel, a relatively stable PHP framework (it has an LTS release). I had worked with it successfully in the past, and we decided it was worth another visit. In order to more fully understand whether it was a worthwhile change, we answered Goldratt’s four questions.

### First, what is the power of the new technology?

Simply put, PHP and Laravel are very mature and operate within a healthier ecosystem (support-wise). Resources like [Laracasts.com](https://laracasts.com/) offer education on topics of varied complexity, and tools like [Homestead](http://laravel.com/docs/5.1/homestead) take a lot of the guesswork out of local development environments. Laravel itself has a number of out-of-the-box features we’ve been missing in the other framework, including queueing, encryption, and payment management.

### Second, what limitations does it diminish?

The skills required to be effective as a PHP developer are generally less specialized and more accessible for our team, which increases each member’s potential contributive ability and enables us to hire employees from a larger, more diverse pool of candidates.

Testing practices with Laravel are well-documented and inherent, whereas the amount of work involved to effectively test in our other circumstance was painful.

We had been constraining our schema and query design to a less-effective ORM, but Laravel’s Eloquent ORM resolves each of our specific problems.

We can also have much more choice with our supporting tools, including the ability to utilize a fully-featured IDE.

### Third, what rules helped us accommodate the limitations?

We performed very involved manual testing prior to a deployment.

Starting development on any given day involved spending several minutes to provision local infrastructure in a specific and error-prone way.

Error handling and logging in the application had to be done in a specific (roundabout and inefficient) manner.

Our data structures were designed according to the limitations of the less-capable ORM.

Batch processes had to be used because setting up appropriate event-driven mechanisms were too effort-intensive.

### Fourth, what rules should we use with the technologies being evaluated?

We should write tests that cover areas of concern and make use of continuous integration to improve confidence in deployments.

The process for development setup should minimize the amount of infrastructure and setup involved.

Exception handling, logging, and collection should be inherent to the system and easy to use.

Data structures should be designed according to logical relationships and proven approaches, not arbitrary limitations.

Events and queuing should drive application behavior and data processing.

>Technology can bring benefits if, and only if, it diminishes a limitation.

<div class="citation">Dr. Eliyahu M. Goldratt</div>

When reality has been defined a specific way for any extended period of time, it becomes an assumption in the minds of those involved. The most difficult thing then about any change is comprehensively adjusting surrounding behavior, which has had the opportunity to evolve to accommodate that assumption and persist in subconscious process. We find it to be true that, as humans, we won’t always make good decisions about a technology by comparing a feature list or discussing supposed “benefits”. Rather, we must additionally map the technology back to behavior and make a determination based on the full context. Goldratt’s four questions helped us get closer to that goal, and they can help you do the same.