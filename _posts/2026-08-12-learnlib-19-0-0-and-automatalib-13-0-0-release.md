---
layout: post
title: "LearnLib 19.0.0 and AutomataLib 13.0.0 release"
date: "2026-08-12"
navbar-group: "News"
author: "Markus Frohme"
categories:
  - "pages"
  - "news"
---

We are happy to announce the release of AutomataLib version 13.0.0 and LearnLib version 19.0.0.

Yes, you read that correctly. Moving onward, we decided to shift the version numbers of both libraries to more prominently communicate breaking changes with major version. Besides these changes, this update provides further notable goodies:

- The [SESE group](https://www.tu.berlin/sese) at TU Berlin contributed a new learner for the novel formalism of *Mealy machines with local timers* (alongside means for conformance and equivalence testing in AutomataLib) as well a new, highly efficient learner for Mealy machines. 
- The [GitHub releases](https://github.com/LearnLib/learnlib/releases) of LearnLib now provide native executables that offer a variety of LearnLib's functionality via the command-line interface without the need for Java or Maven. This is particularly interesting for people who always wanted to use LearnLib in a more scripting-based or AI-based context.
- On the technical side, we modernized our runtime stack by, e.g., moving to Java 17 as the minimum runtime version and adding support for Apple silicon in case of the M3C model checker.

See the respective release notes ([AutomataLib](https://github.com/LearnLib/automatalib/releases/tag/automatalib-13.0.0), [LearnLib](https://github.com/LearnLib/learnlib/releases/tag/learnlib-19.0.0)) for an overview of the changes. We are thankful to all contributors who implemented new features or reported issues.
