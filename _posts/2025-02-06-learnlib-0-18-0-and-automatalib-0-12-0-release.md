---
layout: post
title: "LearnLib 0.18.0 and AutomataLib 0.12.0 release"
date: "2025-02-06"
navbar-group: "News"
author: "Markus Frohme"
categories:
  - "pages"
  - "news"
---

We are happy to announce the release of AutomataLib version 0.12.0 and LearnLib version 0.18.0.

The central theme of this release is *tidying up*. We have moved some classes around to remove split packages in order to support the *Java Platform Module System* (JPMS) and consolidated some of the existing API. This may cause some refactoring, but especially the moving of classes should be easily handled by modern IDEs. Besides refactorings, this release also contains some nuggets. For AutomataLib, non-deterministic systems have received some love with a new Tabakov-Vardi generator as well as a new bisimulation implementation. For LearnLib, the previous `SymbolQueryOracle` has been superseded with the more mature `AdaptiveMembershipOracle` which also supports the processing of query batches. Furthermore, an implementation of the L# active learning algorithm has been added.

See the respective release notes ([AutomataLib](https://github.com/LearnLib/automatalib/releases/tag/automatalib-0.12.0), [LearnLib](https://github.com/LearnLib/learnlib/releases/tag/learnlib-0.18.0)) for an overview of the changes. We are thankful to all contributors who implemented new features or reported issues.

Looking forward, with the release of the next Java LTS version (25) this fall, we plan on bumping AutomataLib & LearnLib with it. This means, for the next release (in about a year), you'll need at least JDK 17, 21, or 25 to build and at least JDK 11 to run AutomataLib & LearnLib. If this causes you any issues, please let us know.
