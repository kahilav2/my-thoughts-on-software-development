# My Thoughts on Software Development
This repository contains a brief text about my thoughts on software development in a company environment. Without further ado, let's begin.

### 1.0 Balancing Speed and Quality in Software Development
##### 1.1 The Trade-off Between Development Speed and Code Quality
As a company developing a software product, our primary goal is to deliver value to society. This often requires a trade-off between development speed and code quality. Taking on technical debt can speed up short-term progress but may slow us down in the long run. Another approach to balance speed and quality is to write simple, reusable code, although this may limit the flexibility of our systems.

Keeping applications simple helps manage overall project complexity. It makes it easier to onboard new team members and reduces the need for extensive documentation.

##### 1.2 Managing Technical Debt
Taking technical debt isn't inherently bad, instead it can be a great strategy, but knowing when to take it as well as managing it can be complex and where mistakes are often made. 

##### 1.3 Technical Debt in "Leaf Node" Applications
Technical debt is more acceptable for less critical "leaf node" applications that other systems don't heavily rely on. Complete rewrites are easier due to typically smaller scope and less dependencies. Also there is the possibility that after initial launch, a leaf node application does not need much modification or maintenance.

##### 1.4 Technical Debt in Core Systems
For core systems, we should always be aware of technical debt and, if possible, make small improvements early and often before it grows uncontrollably. When there's a significant amount of technical debt in a system and new development is added, that new code likely needs to adjust to the existing technical debt. This leads to further accumulation of technical debt, making development time-consuming and difficult. In many cases, the costs of technical debt slowdown will quickly outweigh the costs of taking time for small, early refactors. We need to strike a balance between addressing technical debt and delivering new features.

##### 1.5 Forgotten Technical Debt
It is safe to say that every software company faces the problem of increasing technical debt. It is easy for developers to dismiss the duty for paying up technical debt, and it's quite convenient for developers (and managers) to just "forget" that such thing even exists. That is until it grows so big that it can no longer be ignored. When this happens, for old people, quitting and leaving the debt for newcomers to deal with may become a tempting option. For the company though, the situation can be paralyzing, and therefore, technical debt should be properly managed and not be forgotten or postponed indefinitely.

### 2.0 Knowledge Sharing and Mitigating the Risks of Key Person Dependencies
Another crucial aspect is being prepared for, or at least acknowledging, the risks of people leaving. How do we transfer knowledge? How much knowledge will be lost because a key developer knows too much to teach a new developer in a month? How will we ensure that development can maintain its speed after a key developer quits? Knowledge sharing via code reviews, code simplicity, the right amount of documentation, and everyone taking responsibility in being aware of how much unique knowledge they have are all important. Deciphering how a system works from poor documentation or a messy code base is invariably slow and challenging.

##### 2.1 The Importance of Self-Documenting Code
Also code that documents itself is an important part of migitating the risks of key people leaving. When writing code, think about what kind of variable and function names, comments, and possibly documentation would help a new developer quickly understand your code. Writing code is fast when you know what to write, so adding an extra comment here and there to explain why something is done takes a negligible amount of time. Don't overdo it though; use comments only where justifiable. In my experience, forgetting to write useful comments seems to be a more common pitfall than having a habit of writing too many.

### 3.0 The Debate Between "Over-Engineering" and "Under-Engineering"
Over-engineering and under-engineering are endless sources of debate in any software company. Choosing the right level of engineering is very difficult. We don't have a definite way of knowing at the time of a decision whether the level of enginfeering was correct. Moreover, we can't necessarily infer it from the outcome either. Even if something turned out to be the right level of engineering, it doesn't mean it was the right decision at the time, given the knowledge we had then.

##### 3.1 Challenges in Communication
Effectively arguing with other developers about the right level of engineering is often not straightforward either. How we conclude the right level of engineering involves our previous experiences, programming philosophic values, capacity for abstract, analytic and reflective thinking, our level of intellectual humility, etc. and it can easily be derailed by a momentary lapse in thinking, our personal biases or elephants steering our thoughts (*), personal benefits we might get from certain decisions, and something as simple as not caring much about the work and just wanting to go home.

<sub><sup>(*) as Jonathan Haidt describes in "The Happiness Hypothesis", where our emotional and intuitive "elephant" guides our rational "rider", causing us to justify and rationalize the elephant's decisions after the fact</sub></sup>

##### 3.2 Ever-changing Business Environments
It's also worth noting that the required level of engineering may change over time as the project matures and business requirements evolve. For this reason, an often effective strategy is to initially keep systems small and simple, allowing for fast rewrites or added complexity as we gradually gain more confidence in our business goals.
