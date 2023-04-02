---
title: Summary and Comments on Chapter 1 of "Clean Code"
description: Summary and comments on the first chapter of Robert C. Martin's seminal book "Clean Code". I comment on why I don't like the term "clean code", why I'm cautious with The Boy Scout Rule, and how unmaintainable code is not solely introduced by developers not pushing back on tight deadlines.
date: 2023-03-30
tags:
  - clean code
  - book notes
---

{% include "clean-code-banner.njk" %}

## Chapter Comments

### On “There Will Be Code”

In 2008 R.C. Martin described how code was expected to become obsolete. It’d be generated instead of written, and business people would build products by writing specifications. He attributed it to the growing number of high-level abstractions and domain-specific languages at the time.

A very similar thought exists today because of the capabilities of AI. Some speculate that software developers will eventually be redundant and that business people will create products by describing them to a chatbot.

Some are skeptical of such claims. There has always been a new technology that would take out the intermediary between business and product. But software development is still strong.

R.C. Martin's argument against the idea of code becoming obsolete was that programs can't run on vague descriptions. Machines need detailed and accurate specifications, which _are code_.

Will AI generate effective software from vague language? Will vague language be considered code? Or will vague language not be effective at all?

I’m far from knowledgeable to have an informed opinion, but there’s no doubt AI will have a significant impact on how we build products and approach code.

### On “Bad Code” and “Clean Code”

I find the term “Clean Code” to be evocative. For me, it encapsulates the idea that code is a discipline or a form of craft.

I find the term moralizing as well. It is about “clean” and “dirty”, “good” and “bad”, “beautiful” and “ugly", and “virtuous” and “evil”. The concept rings hollow if developers write "clean code" for virtuosity's sake.

At the end of the day, as mentioned by R.C. Martin, the goal is to improve developers’ efficiency. For developers to be efficient, the code has to be scalable. For code to be scalable it has to be maintainable.

Thus, I prefer the terms “maintainable code” or “scalable code”. They are intent-revealing (_wink_ _wink_), functional, and don’t have the moralizing connotation of good and bad.

### On “The Total Cost of Owning a Mess”

One of the reasons code becomes unmaintainable is because the developers don’t communicate the risks of rushing in work. They don’t want to look incompetent, non-collaborative, or lazy.

Other reason is that not all developers are capable or willing to deliver maintainable code. Team members have different skill sets, priorities, values, and beliefs. Most developers consider their code is immaculate when it isn't. Others won’t even try it because they consider it a waste of time or don’t enjoy what they do. Many lack the experience and knowledge.

Maintainable code is not only a technical issue but also a social one. It requires negotiation, conflict resolution and coaching for teams to agree what maintainable code is and how to achieve it.

As technical leaders and managers, our responsibility is to create an environment where maintainability is a priority.

### On “The Boy Scout Rule”

I am cautious with The Boy Scout Rule.

Leave it better than you find it, but don’t go all the way to clean the whole park.

Improve code that is directly related to the change you want to introduce, and just at the moment you are about to do so. Otherwise, you might be wasting time cleaning code that is stable and might not ever need to change.

## Chapter Notes

The book _<a href="https://amzn.to/3lVl9zx" target="_blank" rel="noopener">Clean Code: A Handbook of Agile Software Craftsmanship</a>_ is for software developers that want to improve their skills. It teaches them to identify and write good code.

### There Will Be Code

As the number of high-level abstractions and domain-specific languages grows, some belief that business people would create software by writing specifications. Software developers would be redundant as code would be generated and not written.

Nonetheless, these languages _are_ code since they provide the requirements for programs to run. Machines are not able to run on vague descriptions. They need precise specifications to run.

> Code is the language in which requirements are expressed.

### Bad Code

Delivering bad-quality code because of rushing impedes development. This results in _wading_ (slowly crawling through code to understand and change it). Is very optimistic to think that bad code will be fixed in the future. It seldom happens.

> LeBlanc’s law: Later equals never

### The Total Cost of Owning a Mess

Messy code slows down development, making future changes non-trivial. The productivity of the team decreases asymptotically towards 0. Management solution is to add more people making the problem worse.

#### The Grand Redesign in the Sky

As productivity falls, management decides to replace the system with a new one. The two systems exist in parallel. The team on the new one has to catch up while the team in the old one continues to add features. When the new system is ready, it is already rotten and unmaintainable.

#### Attitude

Code becomes unmaintainable because developers bend to the manager's pressure to deliver on a tight deadline. It is unprofessional for developers not to put limits when asked to write code that will become a mess and impede development in the future.

#### The Primal Conundrum

Developers know messy code will slow them down but feel pressured to create messy code to meet tight deadlines. _They don't take the time to go fast_.

Developers won’t make the deadline if they introduce messy code. It’ll slow them down. The only way to meet the deadline is to keep the codebase as clean as possible.

#### The Art of Clean Code?

Developers will have to learn to write clean code. Recognizing good and bad code does not mean a developer knows how to write it. They have to tune their code-sense. Code-sense allows the developer to identify how to improve existing code by understanding the techniques and steps to achieve it.

#### What is Clean Code

This are the main ideas of a series of authors who describe what clean code is:

##### Bjarne Stroustrup

Pleasing. Bad code tempts more bad code. Attention to detail. Focused (do one thing).

##### Grady Booch

Readable: exposes the tension of the problem to be solved. Only the necessary.

##### “Big” Dave Thomas

Easy for other people to enhance it. Easy to change. Tested. Smaller is better.

##### Michael Feathers

Written by someone that cares

##### Ron Jeffries

No duplication. Does one thing. Expressive. Tiny abstractions.

##### Ward Cunningham

Predictable, make the language look simple

### Schools of Thought

The book describes a specific school of thought of techniques and practices that the author considers to render clean code. But it does not mean this is the only school.

### We Are Authors

Writing software requires more reading than writing. The ratio of time spent between reading and writing code is 10:1. Developers should write code that is easy to read, which in turn will make it easier to write.

### The Boy Scout Rule

Leave the campground cleaner than you found it. This way, the codebase gets better over time.

### Prequel and Principles

The book _<a href="https://amzn.to/3lVl9zx" target="_blank" rel="nooponer">Clean Code</a>_ is a prequel to _<a href="https://amzn.to/3nAsCob" target="_blank" rel="nooponer">Agile Software Development: Principles, Patterns, and Practices</a>_ (PPP). PPP explores the principles of OO and describes the SOLID principles.

### Conclusion

The book provides the thought processes of good programmers and the tricks, techniques, and tools that they use. Mastery should be conquered by practice.
