# Engineering Principles
This document describes the kind of engineering team we are, and in some cases aspire to be.

It’s important to write it down so we can achieve & perpetuate it.  We do this by using it as the basis for:
* Hiring.  Job descriptions & bands, crafting of our interview process.
* Individual growth & feedback.  Job bands & discussions about opportunities.
* Team growth & improvement.  Goals, KPIs, and associated projects, ceremonies, and time allocation.

Tactically, it can & maybe should cover:
* Best attributes & behaviors.  E.g., we geek about new technologies and generally, learning things
* Habits & general best practices  E.g., we own it in production and ensure we have ways to see if it’s working
* Goals & high level time allocation  E.g., we make time for quality and use that time to do proactive things like clean up code, write tests
* Desired results  E.g., we’re seen as one of the top engineering teams by folks outside Envoy

## Our principles:

* [We maintain high standards](#1)
* [We take pride in doing things right](#2)
* [We act like owners and keep context](#3)
* [We lift each other up](#4)
* [We’re High I/O](#5)
* [We continuously get better](#6)


<a name="1"></a>
### We maintain high standards
* We know perfect is the enemy of good, but we aspire for great.
* We keep things small and simple.  One layer of the onion at a time.  Commits, PRs, tickets, communication.
* Moving fast and decisively helps us deliver value, learn and improve, and achieve quality faster.
* We embrace that change is constant.  The industry, technology, our customers, our business, and our team will change and as such, our code will and should change.
* We build durable habits and practices.

<a name="2"></a>
### We take pride in doing things right
* We feel personally accountable and responsible for the health of our product, code, and systems.
* We make doing the right thing to do easy to do, and invest the time to do it.  E.g., taco, great tests, guilds.
* We leave code better than when we found it
* We care about standards and tech debt, and push back when we need to
* We automate repeatable tasks
* Features are not done until they have long term support (runbook, logging, metrics)
* We deeply understand the importance of creating proper tests

<a name="3"></a>
### We act like owners and keep context
* We love engineering and technology, but we solve for our customers and the bigger teams 1st.
* If we can’t unanimously articulate why we’re doing something, we don’t do it.
* We solve problems we actually have before ones we might.
* We use data to tell us the story.  If we don’t have data, we prioritize getting it.
* We make decisions as a group after informed discussion. Decisions are not dictated from the top, or from the person making the loudest noises, rather they’re based on merit, options, and criteria.
* We look for problems and inefficiencies and find elegant solutions before they become major issues.
* We act with appropriate urgency when the situation calls for it.
* Ship it. We ship relentlessly and fearlessly yet with pragmatism.

<a name="4"></a>
### We lift each other up
* We’re happy when helping others succeed. We prioritize pushing, helping, and teaching each other.
* We make sure everyone has a voice.  We crave diversity of experiences, backgrounds, opinions, ideas, and locations and feel uneasy without it.
* We keep things rational, objective, and shared.
* We work together toward shared goals
* We start with trust in each other and build from there.  We assume good intent and skill 1st.
* We’re humble.  None of us is as smart as all of us.

<a name="5"></a>
### We’re High I/O
* We overcommunicate.  Our PRs, tickets, docs, code, emails, etc. all have enough context to help the reader.
* We ask and listen 1st
* We track and share our work early and often, in service of others

<a name="6"></a>
### We continuously get better
* We live to learn new things and constantly improve our craft, like staying up to date on new technologies, tools, and techniques.
* We’re inspired by what's possible as well as what people inside and outside Envoy know, and eager to incorporate the best.  We use and contribute to open source, for example.
* We try things then learn from them and iterate.  Retrospectives > postmortems.
* We learn by doing, more so than talking
* We encourage cross-pollination of work so we don’t establish gatekeepers of work.
* We aim to not be bored, because we know we’re at our best when we’re not.
* We love and seek feedback.  PRs, data, tests, asking people….it’s all good.





# Our Engineering Principles

As a company we have done well to embrace the principles of Agile and the Lean Start-Up; we have applied them to the way in which we validate learnings related to our products - we iterate, we improve, we measure and, where necessary, we change course. In the context of engineering as a craft, we don't always explicitly apply the same mindset. We should strive to learn, improve and ultimately deliver better quality products in shorter durations. 

The principles below give us the framework to call out what we believe are the foundational elements that ground us, allow us to improve and allow us to iterate and grow. Autonomy without alignment and accountability is chaos; the principles strengthen the aspects related to alignment and accountability. 

There is an emphasis on improving our ability and speed to deliver customer value in production responsibly - while we must focus on improving metrics and the availability of metrics, we must always do so with an awareness of how and where our work is delivering increased value. https://medium.com/@SkyscannerEng/why-engineering-principles-matter-993298f7d792

## We have a clear definition of success for every piece of work

Every task, however granular, needs to be performed with a clear outcome in mind - company, goal, epic, story, task, feature etc. As we commit, we are specific and unambiguous and we should be able to articulate both why we are doing something and when we will be done. The definition includes "done" - see below.


## We ship multiple times a day and deliver customer value week in, week out.

We deliver tangible outcomes regularly and sustainably. We embrace lean principles and fast iterations. We bias towards getting value into the hands of our customers quickly. We have the ability to ship multiple times a day, ensuring we can move fast.


## We use design reviews to validate every significant change

Collectively as a squad, tribe or organisation we have a pool of expertise that we should capitalise on. Design reviews are a platform to share, learn, feed back and ultimately deliver better products. They result in an improved technical design and operability using learning and best practice from others.


## We deliver our products using our defined technology standards  

As our engineering team grows, we need to have the right level of consistency and standardisation. We express our opinions in what we choose to use, ensuring we can then build robust tooling to help support us at scale. This supports multiple facets; internal open source, developer onboarding, service ownership, freedom of movement, rotations and day-to-day operations to name a few. We focus on our customers’ problems over repeatedly making technological decisions, which in turn improves our time to production.


## We peer review every change  

Peer review supports delivery of high-quality changes. It can prevent outages and malfunctions caused by bugs, improves aspects of the code such as reducing tech debt and promotes design consistency, learning and knowledge sharing. Peer review results in a wider level of knowledge within the team in question. Internal services that impact our ability to support our external customers are considered production.


## We cover all changes with automated tests, responsibly

Having extensive test coverage finds defects early and allows us to safely and effectively deliver changes in our code base at scale, something that would not be possible without automation. We also have a code base that, by virtue of the tests, is self documented. We need to balance the dangers of speed with automation coverage to deliver responsibly. As we ship code we should preserve or improve this coverage.


## Our definitions of done include being live in production... responsibly

Customer impact is only realised when our target delivery environment is customer facing (usually production). We optimise our tools, processes and planning for this delivery model. We want to remain accountable for delivering an uninterrupted experience to our customers.


## You build it, you run it

To achieve *World Class Engineering at Scale*, we have moved towards an operating model of *you build it, you run it*. This fosters a sense of ownership among teams who ultimately either run, or responsibly transfer ownership. It should also ensure there is a high degree of accountability for every service/product and that we do right by the traveller/customer.


## We own and are responsible for the data we produce

In order to make correctly informed decisions, we need to treat our data with the same level of diligence as our services. As producers of data, we have a responsibility to ensure the quality of our data and that it is stored and protected appropriately.


## We write with inclusivity, diversity, and accessibility in mind

Our company values inclusiveness in the workplace and we should reflect this stance in our engineering output.


