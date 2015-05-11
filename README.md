# BestPractices
This is the mind dump place to store my favorite software development practices, rules of thumb and quotes (some of them paraphrased by me).
The source of those practices are books, talks, articles and many more.

##Clean code
- Focus on readability (for a sake of other team members), not on perfection.
- If something is too big for your head you cannot reason about it ~Dan North
- Minimize 'Cognitive Load' - thinking too much over a simple thing.
- "See what's really there" - if there is an inconsistency:
    - it may be a special case
    - if it's not then it should be a sign that something went wrong
- Familiarity is not simplicity:
    - you get used to crappiness
    - crappiness is bending your brain
- Sometimes it is worth to step back one step and ask yourself: "What's the dumbest thing you see?" (or ask this question to someone else)

- Complexity is the default state - it grows one day at a time
- Consistency at scale is a daily choice - agree on idioms and guiding principles
- Strive for simplicity - choose tools and techniques that make it easier because "it really shouldn't be this difficult"
- YAGNI:
    - don't commit early unless you know you are going to need it
    - think about event horizon - how soon the dumb thing you did is going to be irreversible
- Push often and commit often - [make the sausage](https://sethrobertson.github.io/GitBestPractices/).

##Testing
- During writing test initialize only what is necessary to make it pass
- Use fluent api / builder to build complicated objects
- **Tests are communication tools**
- **During writing the tests you should still thing**
- Write test instead of debugging
- Clean code principles also apply to tests
- Frameworks can be wrapped to make them testable

##Design patterns
- Do not make new problems only to solve them by applying design pattern
- Singleton is OK if it does only one of those two things at a time: reading or writing
- Strategy and factory are the best friends
- Inject strategy by DI unless it needs to be changed often. Then use factory.
- Decorators can be done by using aspect programming.
- Do not use decorator if it changes completely the behavior of decorating object.

##SOLID:
- Liskov - if you surprise developer - know that something bad happens.

##Planning
- Hofstadter's Law: It always takes longer than you expect, even when you take into account [Hofstadter's Law](http://en.wikipedia.org/wiki/Hofstadter%27s_law).