# About Me

Hi, I'm lemontea, and I am a software engineer. This page is where I try to connect the dot to figure out who I am in my profession.

## My Career

What follows is a simple but tedious story. Forgive me for trying to be exhaustive as some people prefer tl;dr - I simply couldn't resist the temption ;). (Notes to recruiters and people who've read my CV - it's the same material rehashed to have a more personal/idiosyncratic touch)

(Name of Projects/Products are not exact and have been changed to be more generic)

### Act 1 - Captive Portal at a telecommunication company

**Theme: Distributed System, MVC framework, the jQuery era, and Server Admin**

There's a saying, everyone have to start somewhere. I am assigned to maintain a relatively simple subsystem on the Wifi Project Team - Captive Portal for Business Clients (Think shop owners, such as a Coffee Shop or Cafe, who want to provide Wifi to their patrons on premise).

It is "just a bunch of jsp pages connecting to the database and interacting with the wireless router to gate access". Despite its simplicity, it is actually a pretty good training ground in that it is a demostration of the problems and concerns common to all Distributed Systems - issues of consistency, replicating data, synchronisation/race conditions, distributed transactions, CAP theorem, etc. Alas, I did not have access to literature on these subjects and are mostly restricted to books/resources on transactions/replications on traditional database, plus the odd book on temporal logic (an early attempt in my career to dig down to the theoretical underpinning of problems, hoping to gain clarity on the matters). I tried my best to get by using ad-hoc reasoning for all those race-conditions.

This early in my career, I don't even know anything about MVC frameworks for web app, and thanks to my colleague, I am introduced to a book on Java Spring - the first book that I seriously worked through (well, the core part at least).

Computer Science is a young discipline, and a decade is a long time [1]. Back then, frontend SPA framework is still a brewing idea with things like MVVM, Coffeescript, underscore.js and backbone.js. Those I did on my extra-cirrucular. For my day job, jQuery it is.

To the best of my knowledge, DevOps isn't mainstream yet in that year. So I am taught some Server Admin like Linux Shell and Shell scripting, for both operations and ad-hoc website analytics/monitoring/troubleshooting. This later application is an underrated skill that served me numerous times in my career. From here it escalated quickly due to the constantly overloaded server (Budget is limited). From tuning Apache httpd parameters to save the day, to getting lost on configuring a DHCP server, all the way to load-testing using a bare metal server I can physically touch (JMeter + Linux kernel network parameters + struggles to interpret the test result (an early hint at the emerging field of data science?)).

I didn't make it in the end. But looking back, this job is a blessing in disguise - it already included all the major components - Backend, Frontend, Server/DevOps/Infra, and some Networking too. Due to the unconventional nature of this training, as well as my technical immaturity at that age, I still lack perspective and context on many of those stuffs (as I come from a more theoretical/*pure programming* background). But as a course on inspiration, this job have fulfilled its purpose.

### Act 2 - R&D Prototyping of a Network Coding scheme

**Theme: Low level programming, P2P system, and reading research paper to turn it into reality**

**Extra curricular activity: Advanced Programming Language, NoSQL and Big Data, Code Refactoring and other Good practise**

Siezing on an opportunity, I took a change of scene to this job. This is a special one in that it is the only job that doesn't involve coding the same CRUD/web app stuff. Another notable point is that I am placed in a team that works like a startup, embedded inside an academic research enviornment (Later on I took on what looks like an internal consultant role working cross-team, and unbeknowest to me, this is a foreshadowing).

The project is an attempt to commercialize an academic research that constructed a novel Network Coding scheme. Serendipitously, a colleague have an idea to do a startup on P2P technology, and someone come up with the idea of using the novel Network Coding Scheme to boost P2P performance.

Since I have a double degree in both mathematics and information engineering, I am naturally slotted into a role of writing the low level library implementing the Network Coding Scheme.


Due to the rather niche domain of my job duty, there's plenty of downtime. And so begun my traditional of pursuing *extra-cirrucular activity* (or more formally, professional development) - learning the latest trend on technology, innovations, ways of thinking, etc.

Coming from a *coder*/*programmer* background, I was initially more attracted to try to learn multiple programming languages at first, in order to keep up with the Jones (I heard, back in my undergrad days, that *those guys* in CS learn a few programming languages *as a minimum* - to someone who only know C/C++ initially, this can be intimidating). In that year, various *Hacker style languages* gained popularity (such as Python and Ruby), so my choice is to avoid repetition/mainstream languages. Luckily, I heeded an advise I found online that "you should learn programming languages in different paradigm, with very different features/philosophies" and that "each new programming language you learn should give you a new way of thinking". By luck, I stumbled upon both Haskell and Lisp (arguably representing two of the most powerful lines of thoughts - Advanced Static Typing, and "Code is Data" aka "Homoiconicity"). Lisp especially have been a lasting influence on my journey, guiding me towards a more light-hearted, artistic view on programming. Pragmatically, it led me to Chapter 4 of Practical Common Lisp, and then SICP, and later on, Rich Hickey's talk on Clojure.


### Act 3 - Introduction to Enterprisy, Event-Driven Architecture

**Theme: Message Queues, more concurrency bugs, Early day SPA frameworks, Internal Wiki and tech sharing**

**Extra curricular activity: Combinatorial Optimization**

Thus far I've got a sample, a taste of working in software. I know I need to "get serious" in some way for my next step - whether it is scaling up in terms of complexity of technique/practise/organization, codebase size, or even just the size of the server, anything. And so an Enterprisy job seems like a reasonable choice.

And man did I get the answer. I learned, for the first time in my life, how large scale gives you the affordance to simply throw resources at a problem that, were it to be done by any smaller companies, would be considered insane (and rightly so). They've got a whole bunch of internal software frameworks. (If you've heard anything about FAANG, this would be no big deal of course, so forgive me - me at that time is someone who've never seem the world)

Let's get back to the software. It is some kind of logistic company, and uses Event-Driven Architecture to deal with the massive amount of data coming from sensors in the world attached to various things (sorry for being vague). My team is responsible for a component that process these events in a centralized manner, even when the events can be related to many different "departments" - in other words they are quite heterogenous. As such this component sits at the center/intersection of different, sometimes conflicting business processes/flows. To make matters worse, your usual concurrency bugs are fulfilled as promised, and the company is in the middle of a migration strategy that involves first running both the new and old systems in parallel (using replication/mirroring to sync the data), and then switching the primary to the new system. The combined force of these pressures is just too much for me and I quickly crumbled - ironically not really on the technical side of things.

But I do learn a few lessons. First - concurrency in distributed system is a difficult problem, and by this time I am beginning to sense that this is going to be a recurring theme in my career (comparing notes with similar issue in my first job). By repeatedly thinking about this issue in general in my head, I am coming to the sense that a more systematic approach is necessary. Second, Legacy system is common, and how to modernize/migrate/refactor/do anything to improve is going to be a difficult, but worthwhile problem. This planted the seed for me to go out and search for new perspectives in the future. Third, it is becoming clear that the human factor in software engineering often play a decisive role, and as much as I am a "technical person", I know I can't completely ignore it anymore.

Continuing on, even though this job is the shortest one in my career, there are other topics "covered" too. I get introduced to a version of the 3-tier architecture in its full manifestation, complete with web service call and EJBs. I worked on various tasks to generate reports from database, or to migrate data, etc. I get to see production deployment (still no modern DevOps though) and limiting developer access to production, plus how tedious it can be to extract logs. I also used an early day SPA framework in my job, one that unfortunately attempted to replicated class-based OOP like Java in Javascript. I also pushed some code to its absolute limit to achieve what would otherwise simply be impossible - a move that I regret later.

In many ways, this short stint is a "preparatory job" for the real job next - aside from the above, technically I got exposed to some pretty heavyweight Java, and without my knowing it, I've actually adapted and gained the ability to pick up complicated libraries/frameworks, and navigate software ecosystem in general. These skills would propel me from survival mode to something that's more autonomous in the future.


### Act 4 - Legacy System Makeover, Distributed System, Glue, and Technology Trends

**Theme: How to modernize legacy system, RESTful API, Unit testing, Complex Distributed System, AngularJS, Payment Gateway Integration, PoC/Technology Prototyping, Technology Seminar, Algorithmic Challenge, Security, Cross-team and cross-organizational collaboration, Mentoring**

**Extra curricular activity: Reinforcement Learning, Containers/Kubernetes, Ansible, Vue, Clojure, Microservice, GraalVM, Research in Programming Language Theory, Enterprise Architecture and Design Pattern**

#### Generalities
By the time we get here, the list is getting real long.

My job duty have expanded in scope unofficially - being responsible for a whole project, and taking ownership over a whole (multiple?) product lifecycles. At this point, cross-team collaboration has already become a background fact - in fact I find myself needing to work across the whole organization, and occasionally, *across organizations*, in order to carry out my job duty successfully. And all these while officially only carrying the title of *(Senior) Analyst Programmer* [2]. I would like to give special thank to the company for giving me this leeway - I believe this wouldn't have been possible at all in more Enterprisy settings where the regimetation and siloing is more strictly enforced.

Due to my gradually gaining experience and technical ability, as well as being in a politically less powerless situation, I find myself, for the first time ever, having some sort of organizational *citizenship* and *agency*. *Citizenship* refers to the idea that one's personal interest is aligned with that of the company and so act for the long term common interest. An example would be taking initiative to try better ways of doing things, or implementing new internal tools/infras to make everyday life better. *Agency* refers to the ability to take those initiative, instead of always taking order from higher up passively. Again, this is only possible due to a lucky confluence of many factors - a small company, with transparency in most aspects, management being too busy sometimes to micromanage everything, to name a few. (TODO: add some warning)

#### Legacy system modernization
My first assignment is to modernize a legacy system by implementing a RESTful API in parallel, sharing the same underlying database. As part of my research, I come across Martin Fowler, and I am blown away by just about everything he says - in between Enterprise Architectural Patterns, CQRS (Command Query Responsibility Segegration), Event Sourcing, DDD (Domain Driven Design), DSL (Domain Specific Language), Microservice, and his thoughts on Legacy system replacement efforts, I would be plentifully supplied with ideas to munch over for many years to come.

After completing the first assignment and having it deployed to production, I was then assigned to the team for maintaining the Cinema's Ticketing System. It is a complex distributed system with various booking channels each being their own, largely autonomous, subsystem. Aside from the usual rounds of concurrency issue, here there is additional consideration of replication, asynchronity, and the consistency-availibility tradeoff during partition event (made more subtle considering the need for walk-in booking in physical sites to take precedence). Thankfully, most bugs end up being resolved successfully. In future, this system would become the basic example I use as a reference while learning the principles of distributed systems from books and papers.

Another aspect of this system is its sprawling nature - it spans across departmental and organizational boundaries with many integrations against third party system. Using the tracing skills I've acquired over previous jobs, I gradually gained a holistic understanding of each of its pieces. Sadly, after several changes of managements, it eventually become clear that the complexity have exceeded any economic sense in trying to refactor it and that a business decision was made to exit from this market. Although some subsystems are only rewritten from scratch instead of being removed, I was not assigned to this task.

#### Internal Research/Tooling/Consulting

From time to time, there is a need to implement something using new or unproven technologies or technique. I help out by writing Proof-Of-Concept and/or prototypes. This invovles emerging web API/standards.

During downtime in between tasks, I look at the existing state of affair in the company and conduct experiments on tech, good practise, etc. In one instance, I managed to implement an internal tool to automate away some repetitive maintainence tasks.

As the company have a relatively flat hierarchy and open culture, I also exchange views on technology trends and good practise with colleagues regularly. When called for, I advocate alongside colleagues for bringing in certain good practise that we believe are beneficial to the company. In one instance, I called into attention potential security vulnerability of other team's code.

#### Privacy compliance

The next big project that I am responsible for is to modify an existing legacy system so that it respects end user's privacy. I made a painstaking analysis of the current situation as well as the system flow, and found out that satisfying this requirement is much harder than expected due to the constraint of being unable to refactor it - I have to apply duct-tape so to speak while not modifying the overall structure of the codes, which was very messy.

This means that I have to be extra careful, as this make any attempt at a close-to-mathemtical proof that the modified system does respect privacy almost impossible to do. Nonetheless, as this task is considered top pirority by management, I persevered and marched onward. Taking lessons from some of my failed projects back in College days due to over-ambition and the lack of an iterative approach, I tried to walk the thin line between being rigorous enough to not let minor issue that could still completely jeopardize privacy slip away, versus not making any progress due to over-insistence on perfection.

At the end of the day, the task is said and done. Luckily, it is only an interim measures as it would later be completely replaced.

#### Client Projects

During the later phase of my tenure at this company, I am reassigned to two different "Client Projects". This company have both an in-house and a vendor role, helping client implement custom softwares.

In the first one, I played a minor role as an Individual Contributor (IC) doing a few feature tickets in their sprint. This is the first time that I actually did modern frontend work using AngularJS plus webpack. I studied version 1 of Angular on my own research, and the company hired external training for version 2 of Angular.

In the second one, I become the main developer responsible for meeting client demands alongside another junior colleague. In a relatively short amount of time, I have to understand enough of the whole system to become effective, as the features/changes demanded is relatively complex while also being on a tight deadline.

It is here that the various "thread" we have previously come together:

- My system level skill (together with knowledge of Java) become crucial to help me stay afloat
- As the client is a large enterprise, and the system involves integration against their system, access to insider knowledge of their system and documentation become critical. Taking experience working with external/third parties in previous assignment, I navigated their bureacracy and helped their contact person understand their own system better. At the same time, I also help to manage expectation and assuage any fear they may have of us being unable to deliver.
- I mentored my teammate by providing both general CS knowledge, as well as specific instruction to cover weak spots. My teammate learned, improved, and helped contribute to the project during a critical period, and as a result we meet the deadline against the odds.

#### Extra-curricular

I have been keeping an eye on technology trends throughout these jobs, and in these years it become clear to me that the industry is developing substantial depth. Therefore, I made it part of my career strategy to try to systematically explore emerging topics and catch up.

**In the area of DevOps**, I have been motivated by 1) the relatively antiqued practise in all companies I've worked with thus far in terms of server administration and production deployment, and 2) the lack of, and difficulty in, introducing good practise (even the basic Unit test + Refactor + CI/CD trinity of virtue have been an uphill battle **even for orgnizations that officially recognized their importance and made it an official policy to try to implement them**).

While I forgot exactly when was the first time I got in touch with the idea of container, I liked it a lot. Strangely, although I remember learning it relatively easily outside my job duty, the idea of containerising the systems I am assigned to in my job didn't occur to me - despite me "selling" these ideas to my colleagues in view of the problem with using long term virtual machines. Perhaps this is due to another idea, IaaC (Infrastructue as Code) also taking up my mental bandwidth. (Confession: I have secretly played with using Ansible to administer some development server at company)

Kubernetes also went up in my radar, at first at the edge. However, as I keep coming back to it, I growed more liking for it later on.

Regretably, there is a missed opportunity here. After my resignation from this last job, I was informed that the company has a plan to introduce modern DevOps practises. I wish the company success in this initiative.

**In the area of System Architecture**, I have been motivated by being bored with the MVC architecture and wondering if there is alternatives. Perhaps more responsibly, my constant struggle with legacy system and code complexity have led me to consider the idea that MVC isn't always the optimal architecture for complex web app. Taking inspiration from Martin Fowler (see above), and recalling my brief exposure to the Event Driven Architecture in the last job, my study eventually led me to Microservice. Although they are different things, I am stimulated by seeing many new ideas being used togehter (in short: Message Queue + Async pattern + CQRS + Event Sourcing + Microservice is an interesting combo. I would see an evolution of this idea later on too).

**In the area of Programming Language**, this have been a long tradition in my career. Originally motivated by my struggle with code complexity, it have evolved into a passion for grasping universal principles of programming language (perhaps echoing the Polyglot movement. Alas, it didn't last long - turns out linguistic barrier is real. However, a variant of this idea known as "Polyglot persistence" would continue to influence my thinking). I think this have to do with the fact that once you managed to learn a few programming languages, each from a different paradigm, successive new language become easier to learn.

That being said, I simply love Lisp. While Haskell is cool with its close alliance with pure math, I like the aesthetic of Lisp more in its simplicity and uniformity. By contrast, the dominant language I use in my career, Java, is infamous for being verbose and Enterprisy. You can imagine how overjoyed I was when I discovered Clojure - A marriage between Lisp and Java. Its design also have all the elements I like - functional programming, and nice, simple constructs for treating concurrency in a principled manner. (No, it is not invention out of thin air - it have taken lessons from the CS literature a few decades ago, back in the golden age. This point makes me appreciate it even more)

**Finally, in the area of AI**, hearing the news of AlphaGo, I used my personal time to study reinforcement learning.

### Act 5 - Back to the Basics, Quest for a better way, and it takes a village to raise a child


In my previous incarnation of a career, a meta-theme that gradually emerges is one of increasing *Citizenship and Agency* - instead of being just a Corporate drone carrying out order, I yearn for a place that we can care about, and care enough to Garden it. It turns out the same "game" plays out on a larger scale in the open world.

A second meta-theme is my constant struggle for *a better way*. It is a tragedy to see the same disaster over and over again. It is even more of a tragedy if you think you know of a way to stop the cycle, but are powerless to implement and effect change.

However, of the two meta-themes, I ultimately decided that the first is more important, and this comes as a result of me going back to the basics.

#### Fundamentals: Computer Architecture, OS, and Algorithms for Concurrency, Distributed System/Big Data, and Blockchain


#### Backend: The problem of Database and Architecture


#### Frontend: Struggles of Javascript, SPA, and toolings growing up


#### More Frontend: CSS, Web Component, Design System, and HTML5 API


#### Special: Blockchain/Web 3, JAMStack, and future architecture


#### DevOps and Cloud: From Kubernetes to Openstack, iterating understanding


#### AI: Having fun with math, and some surprise in morality and ethics


#### Endnote: Seeing the outside world



[2]: I started out as an Analyst Programmer, and eventually get promoted to Senior title.
