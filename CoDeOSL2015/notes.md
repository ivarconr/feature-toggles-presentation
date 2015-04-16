From:

http://swreflections.blogspot.no/2014/08/feature-toggles-are-one-of-worst-kinds.html

The plumbing and scaffolding logic to support branching in code becomes a nasty
form of technical debt, from the moment each feature switch is introduced.
Feature flags make the code more fragile and brittle, harder to test, harder to
understand and maintain, harder to support, and less secure.

# Feature Flags need to be Short Lived!
=> main purpose of toggles is to perform release with minimum risk, once
release is complete toggles need to be removed.
=> Feature Flags are Technical Debt – as soon as you add them


Release toggles are supposed to make it easier and safer to push code out.
You can push code out only to a limited number of users to start, reducing
the impact of problems, or dark launch features incrementally, carefully
assessing added performance costs as you turn on some of the logic behind
the scenes, or run functions in parallel. And you can roll-back quickly by
turning off features or optional behaviour if something goes wrong or if
the system comes under too much load.
=> dette får man ikke til med feature brancher! All or nothing approach!


=> Strategies makes it harder to test features. Harder to know what is actually
going on in production.

# Use Feature Flags with Caution
- Minimize your use of feature flags for release management, and make the implementation as simple as possible.
- Review flags often,
- Once a feature is part of mainline, be ruthless about getting it out of the code base as soon as it isn't used or needed any more.
- Recognize and account for the costs of using feature flags, especially long-lived business logic branching in code.
