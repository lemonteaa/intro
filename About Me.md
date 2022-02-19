# About Me

Hi, I'm lemontea, and I am a software engineer. This page is where I try to connect the dot to figure out who I am in my profession.

## My Career

What follows is a simple but tedious story. Forgive me for trying to be exhaustive as some people prefer tl;dr - I simply couldn't resist the temption ;). (Notes to recruiters and people who've read my CV - it's the same material rehashed to have a more personal/idiosyncratic touch)

(Name of Projects/Products are not exact and have been changed to be more generic)

(It turned out to be even longer than I expected. At this length, I don't realistically expect anyone to read all of it - just pick sections you're interested in I guess.)

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

However, of the two meta-themes, I ultimately decided that the first is more important, and this comes as a result of me going back to the basics. But first, we must go over the search for a better way thoroughly before that becomes clear.

#### Fundamentals: Computer Architecture, OS, and Algorithms for Concurrency, Distributed System/Big Data, and Blockchain

Although I have some background knowledges in CS, as my career progressed, it become clear that a more in-depth and systematic investigation is needed to "close the gap" on several questions I have. Some targetted choice of books help. For the rest I find the need to dig down and search the Internet opportunistically. Here's how it mattered:

- Knowing the details of computer architecture beyond the basics of von Neumann architecture - things like cache and virtual memory - lay the groundwork for clearing some confusion on how OS works [3].
- In turn, knowing how OS interface with the hardware provided the knowledge and confidence needed to actually learn Cloud computing technologies more deeply.
- Knowing the low level also helped me to understand the fact that *concurrency issue is a cross-cutting concern*: it spans across the whole tech stack so to speak.
- Perhaps more importantly, on a meta-level, I begin to realize that the design of computer hardware and software is a mutually dependent, symbiotic process.
- The theory of distributed algorithms/formal models helped clarify issues in concurrency (e.g. The concurrency model of a CPU). It also become the basis for further learning in Big Data Systems.
- And last but not least, I am lucky to have learned a body of interrelated ideas spanning different topics all in the right order: from Raft algorithm, to replicated state machine, to the append-only log architecture of backend proposed in "Designing Data Intensive Application", to blockchain.

On another note, special mention to [The morning paper](https://blog.acolyer.org/). Although it have gone into hiatus, the quick review/summary it has of many important papers in CS have helped a lot (in no particular order and not exhaustive):

- [A Survey on Reactive Programming](https://blog.acolyer.org/2015/12/08/a-survey-on-reactive-programming/)
- [Opening the black box of deep neural networks via information](https://blog.acolyer.org/2017/11/15/opening-the-black-box-of-deep-neural-networks-via-information-part-i/) But see also [this](https://blog.acolyer.org/2017/11/24/on-the-information-bottleneck-theory-of-deep-learning/)
- [Formal foundations of serverless computing](https://blog.acolyer.org/2019/11/18/formal-foundations-of-serverless-computing/)
- [The seven tools of causal inference with reflections on machine learning](https://blog.acolyer.org/2018/09/17/the-seven-tools-of-causal-inference-with-reflections-on-machine-learning/)

Some other papers (also not exhaustive):

- [Revisiting the Paxos Algorithm](https://www.microsoft.com/en-us/research/publication/revisiting-paxos-algorithm/)
- [Collapsing Towers of Interpreters](https://www.cs.purdue.edu/homes/rompf/papers/amin-popl18.pdf) (Theory underlying [GraalVM](https://www.graalvm.org/). See in particular [this listing](https://github.com/oracle/graal/blob/master/docs/Publications.md), and the paper [Practical Partial Evaluation
for High-Performance Dynamic Language Runtimes](https://chrisseaton.com/rubytruffle/pldi17-truffle/pldi17-truffle.pdf))

#### Backend: The problem of Database and Architecture

My career have so far mostly focused on this area, so it is reasonable to take a step back and look at it more carefully. Summarizing previous experience, I have narrowed down my focus down to two points:

1. You're stuck with either using traditional RDBMS, or some NoSQL solution. For the former, it becomes the "center" of the universe in the whole application/system. Everything of substance ultimately goes into, or out of, the database - the rest are really just sugar-coating/gold-plating. Because of this SQL and schema are everything, but they are tedious to write, not composable/reusable (embedded solutions like stored procedure has their own problem - which is that their language is stuck in something like COBOL), and you have got the *object-relational-impedance-mismatch* problem, which is so hard to solve that it has been called the ["Vietnam of Computer Science"](https://blog.codinghorror.com/object-relational-mapping-is-the-vietnam-of-computer-science/). If you use NoSQL on the other hand, it often ends up being even harder to write correctly as you're now responsible for any (weaker) consistency model you want to ensure, and application become somewhat brittle as the DB access is now more tightly coupled to the exact situation in the app. Moreover, the lack of a standardized language increases risk of vendor lock-in.
2. Architecture are too expensive to design, too top-down in its role in the Software Development Lifecycle (SDLC) (even in Agile process), and often lack clarity. There is also the problem that education in this area haven't been as widespread as other topics in programming, creating a false stereotype that the traditional MVC/3-tier/3-layer is all there is (this may have improved somewhat in the intervening years with the emergence of cloud, Microservice, Serverless/Lambda, the Edge, etc).

Although I'd like to be as systematic/logical as possible, the fact is, these two are interconnected problems that make software difficult to write and maintain as it scales up due to complexity and a misfit in mental model. So it would occur that the process of exploring a solution is also more nonlinear and intuitive than using pure logic. As I read new ideas from smart people, pieces of the puzzle would connect with some hints of those same idea/theme from piror point in my career (that I already mentioned in the sections above), and eventually all threads would come together.

It turns out that the higher level philosophy is the key. In this regard some pivotal pieces I've read/seen include:

- Rich Hickey's ["The Language of the System"](https://www.youtube.com/watch?v=ROor6_NGIWU) talk, in which he proposes a view of system architecture as ideally being composed from generic, reusable elements.
- Bret Victor's ["Inventing on Principle"](https://www.youtube.com/watch?v=PUv66718DII) (See also [Learnable Programming](http://worrydream.com/LearnableProgramming/))
- Other: Anything by Christopher Alexander (like the [Timeless way of Building](https://wiki.c2.com/?TheTimelessWayOfBuilding))

While there is no absolute, my thinking in this area has been guided to go back to principles. Decomposition and more importantly, decomplecting (Terminology by Rich Hickey) concepts that are in fact orthogonal but are misrepresented as one thing is the main tool I use. On the other hand, it is also important to maintain fluidity and openness - especially to real world messiness/complications.

Going back the problems, here's my analysis:

- In Database world, one should decompose the features offered by a system. Taking RDBMS as example:
  - Relational *data* model - ideal if there are multiple competing view of the same data with no clear winner. Ironically Domain-Driven-Design solves the same problem while allowing you to deal only with aggregate, which is to say objects.
  - ACID *transaction* semantics - Provide strong consistency by sacrificing availability [5]
  - Rigid *schema* - great if your system has stabilized and you want predictability, otherwise not (see also: static vs dynamic type religious war, Zach Tellman’s talk)
- In a similar vein, when it comes to the requirement placed on a system, there is often a conflict between *performance* and *easy mental model*.
- Inspired by the [C4 model](https://c4model.com/), I prefer to think about System Architecture as not one entity, but three complementary views: the Conceptual, the Physical, and the Code level.

And then, post-hoc justified, this is how my puzzle pieces fit together:

Starting with the base of Event-Driven Architecture with CQRS and Event Sourcing, I then go on to read "Designing Data Intensive Application". Before this book, I already know about Kafka and how interesting [the append-only log abstraction is](https://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying). This is also related to the Raft consensus algorithm with the Replicated State Machine paradigm. Indeed, the book do talks about them, and to my joy, in the final Chapter it proposes an Architecture for distributed system based on pushing transactions onto such a log, and have replica replay the log while executing the effect.

And then we have database like [Datomic](https://augustl.com/blog/2016/datomic_the_most_innovative_db_youve_never_heard_of/) and later on, [XTDB](https://xtdb.com/). (It is [renamed from Crux due to legal issue](https://www.xtdb.com/blog/crux-to-xtdb-rename/)) - the later one is essentially an implementation of this proposed Architecture in the form of a Database.

I then separated issues in Database into the underlying execution method, and the language/abstraction/interface it gives to the programmer. On the later part, I find the [RDF triple](https://en.wikipedia.org/wiki/Semantic_triple) data model and the [Datalog](http://www.learndatalogtoday.org/) query language to be much more pleasant to work with than SQL. [6]

Note that due to replication, while the log is regarded as the ultimate source of truth of the data, there is nothing preventing one from having additional database (likely in other paradigm) derive new data, and store/present them in a way that fit other requirements. That is, polyglot persistence.

In fact, this circle of ideas can be pushed even further. In the book "Designing Data Intensive Application", the proposed Architecture is actually an end-to-end one spanning *both* frontend and backend. Outside of this book, similar idea is raised by blog post like [this one](https://tonsky.me/blog/the-web-after-tomorrow/). Here it would appears that GraphQL and Query Subscription (say in Firebase) would be some building block one can use.

Outside of this core, other ideas:

- [The Clean Architecture](https://www.dandoescode.com/blog/clean-architecture-an-introduction/) (also called the Onion/Hexagonal Architecture) (fit well with functional programming) (But see also [this](https://www.jamesmichaelhickey.com/clean-architecture/) - in short mental flexibility is needed. Maybe bring in the C4 view plus ideas in Microservice?)
- Some things may change when you switch over from an object oriented language to a functional one. Such as replacing the [SOLID principle](https://clojurefun.wordpress.com/2012/09/24/the-vapor-principles-for-functional-dsl-design/).
- There's actually a third problem I also explored but didn't mention as it's more technical/low level - dealing with Business Transaction. A combination of [long running operation in API design](https://cloud.google.com/apis/design/design_patterns#long_running_operations), [Saga and compensating transaction](https://microservices.io/patterns/data/saga.html), [Transactional outbox](https://microservices.io/patterns/data/transactional-outbox.html), and [idempotency key](https://stripe.com/docs/idempotency) seems to be the right mix that answered it satisfactorily for me.

#### Frontend: Struggles of Javascript, SPA, and toolings growing up

Although I'm interested in this area, I've had not much of an opportunity to actually do work using up-to-date tech. I think this have to do with the fact that Javascript and its surrounding ecosystem is still too young and exploring the "right way" to grow. So it is inevitable to have some false turn and dead end (Which is pretty much every frontend tech I've used up to this point, even including Angular in some sense as it is rapidly overshadowed by React [4]. I'm simply unlucky in this department, as I shrugged to pretend my unluckiness field doesn't exists.)

Joking aside, in the years before, the churn rate of JS libraries/frameworks/approach is simply crazy (see [this article](https://hackernoon.com/how-it-feels-to-learn-javascript-in-2016-d3a717dd577f#.t3fn4vrpb)). So one could also argue the other way that I am actually lucky to only begin seriously learning this after the dusts *apparently* have mostly settled. E.g. Webpack is battle-proven and stable and a "safe choice", and most importantly there is a default that hide all the casualty of the last war under the rug. (Flame war I mean. Grunt vs Gulp, bower vs npm, AMD vs CommonJS (before ES6 module is a thing)... with this many point of divisons, I think we are all doomed. Wait, we also have SystemJS vs Webpack, and this kind of debate is kind of revived with the rise of the [next gen build tools](https://css-tricks.com/comparing-the-new-generation-of-build-tools/). Opps.)

Anyway, long story short. In a few iterations I learned modern Javascript, complexities hidden by the tooling (still learning on this part though), and React. I actually played with Clojurescript first though, going through reframe and shadow-cljs, and just stopping shy of managing to grok fulcro (Sorry).

A good thing with frontend is that the "hardware requirement" for hosting is way less than backend, making practise project more possible.

#### More Frontend: CSS, Web Component, Design System, and HTML5 API

Going even lower level. One thing that have bothered me is the deceptive hardness of CSS. Sure, the basics look simple, but once you try to do serious layout work, and find out that modern practise doesn't use `<table>`, all hell break loose - `div`-ception *style*. (Yes, I write html back in school days with a book on Dreamweaver in my room)

This is further confirmed by that one time I need to fix problems in layout in some company website. The night spent debugging is long, tedious, and just feel nasty in general - even worse than concurrency bug in some way.

Even excluding layout, the modern webpage have so many fancy eye-candy and effects (transitions, animations, font, scrolling...), that the number of CSS property exploded.

All these took me to a point where I say *enough is enough*. I want to find out a better mental model for working with CSS, expecting a different paradigm than all the general purpose programming languages I've seen before. So begin my journey.

**Modern CSS**


**Just what is a Design System?**


**Web is an evolving platform**



#### Special: Blockchain/Web 3, JAMStack, and future architecture


#### DevOps and Cloud: From Kubernetes to Openstack, iterating understanding

One thing I've learned in my career is that the difference in technological capabilities across different companies can be *tremendous*. Some companies may be on the cutting edge of DevOps and Cloud, doing things like Observability and Service Mesh, and adding global CDN, and using serverless in select components. Meanwhile, some companies may be stuck with using VM for their workload struggling to even just containerize it. A repeat theme is that technologies build on top of each other, hence it seems that there is a kind of [Matthew Effect](https://en.wikipedia.org/wiki/Matthew_effect) at work.

Interestingly, I forgot the exact timeline of myself being able to work with containers. It does come somewhat naturally without explicit learning, and I have felt it to be a productivity booster and easy "win". Strangely though, I didn't incoporate it in my day job. Kubernetes on the other hand is a different matter. Although I also like its idea, its learning curve is, at least initially, higher. The yaml syntax is clunky to work with to say the least.

In an effort to gain hands-on experience in this area, I started out trying to install Openstack on my dev machine using a VM. Manual installation is quite difficult taking me a long time, and even though it worked in the end, I have difficulty in installing the less used/non-core components. The relatively heavy hardware requirement also forbid me from doing extensive experimentation for some time.

On the next round I go back to Kubernetes. While learning its basic command, like `kubectl create deployment` or `kubectl apply`, is "easy", getting access to deeper aspect is harder. Mainly, I don't know where to start.

This would get solved through some serendipity. First I come across a course on Kubernetes Security on Linux Academy. This has the side effect of revealing some of Kubernetes's underlying component (`kube-apiserver` and `etcd` as the backing store etc). Then, in trying to use some cloud based, shared Kubernetes cluster's namespace, I did research on ingress, and this is the beginning of me discoverying kubernetes's vast ecosystem.

Later on I would stumble across an article that explains kubernetes networking internal. Again, lucky to be in the right place at the right time - I have studied more OS and learnt just enough about Linux Networking Stack so that the article "clicked".

Eventually, with learning about vxLAN, and clearing some previous confusion I had on Computer Networking and how Router works, I then come across a blog that explains Openstack internal in some depth. This re-ignited my interest in this topic.



#### AI: Having fun with math, and some surprise in morality and ethics


#### Endnote: Seeing the outside world



[2]: I started out as an Analyst Programmer, and eventually get promoted to Senior title.

[3]: Traditional university course on OS seems to underemphasize the practical aspect of actually interfacing with the hardware, which is a bit strange given there is a separate course on assembly programming. Perhaps the problem is that the very old Intel 8086/8088 is used for teaching. While it is cool to mention the backward compatibility of modern x86 CPU all the way back to this grandfather, the lack of modern extensions/facilities like protected mode/paging and VT-x prevented me from connecting the dots until this point.

[4] However, in recent survey AngularJS is making a comeback somewhat. It is important to keep in mind Gatner's Hype Cycle and the fact that popularity is a rather unreliable thing - it is going to ebb and flow always.

[5] Although CAP theorem is a quick way to summarize the situation, it is somewhat of an over-simplification, it's too easy to misinterpret, and reality is more complicated - that's why we have things like [CALM theorem](https://databeta.wordpress.com/2019/01/08/an-overview-of-the-calm-theorem/), [PACELC](https://ardalis.com/cap-pacelc-and-microservices/), or, if you want something else entirely, the [FLP impossibility theorem](https://www.the-paper-trail.org/post/2008-08-13-a-brief-tour-of-flp-impossibility/).

[6] There's still quite some room for innovation simply by being well-read in classical literature and then recycling good ideas from the Early days of CS that end up not becoming mainstream today due to a confluence of economics, luck, and physical constraints. See e.g. [this](https://www.karimarttila.fi/clojure/2022/01/13/datalog-exercises.html).
