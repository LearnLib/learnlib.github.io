---
title: "LearnLib 0.15.0 and AutomataLib 0.9.0 release"
date: "2020-02-06"
categories:
  - "pages"
  - "news"
---

We are happy to announce our new (annual) releases of LearnLib and AutomataLib.

This release contains mostly updates to AutomataLib. Among the main new features are a new parser for DOT files, a parser for LTSmin-based LTL formulae and a new facade for Paige-Tarjan based automaton minimization.
We were also able to provide some QOL improvements and fix some bugs due to feedback from the community.

There are also some goodies in it for LearnLib.
For one, the `W(p)MethodEQOracle`s now allow you to dynamically address the hypothesis size over the learning process and second, the concept of inferring partial automata (i.e. not querying the `SUL` if certain inputs are not possible) has now been refactored to a `SUL` filter, which allows you improve query performance with any of the existing active learning algorithms.

For details, see the release notes of [LearnLib](https://github.com/LearnLib/learnlib/releases/tag/learnlib-0.15.0) and [AutomataLib](https://github.com/LearnLib/automatalib/releases/tag/automatalib-0.9.0).
