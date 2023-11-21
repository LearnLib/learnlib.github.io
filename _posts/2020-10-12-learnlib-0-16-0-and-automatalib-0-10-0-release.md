---
title: "LearnLib 0.16.0 and AutomataLib 0.10.0 release"
date: "2020-10-12"
categories:
  - "pages"
  - "news"
---

We are happy to announce our new releases of LearnLib and AutomataLib.

This one is a little bit of a smaller release, because some of our projects progressed slower than anticipated due to the COVID-19 pandemic.
To not keep you waiting, we therefore decided to publish the goodies we had so far a little bit earlier.

The most notable changes in AutomataLib are a new implementation of our `DOTParser` which is now self-written and therefore tackles an issue of the previous third-party parser and the support for GZIP'ed input streams across all deserializers.

Regarding LearnLib, we have cleaned up some of the parallel oracle code which now offers convenient builders for various `SUL` (plain, observable, state local input) and `MembershipOracle` (plain and omega) types.
Furthermore we provide a new `StateLocalInputSULSymbolQueryOracle` wrapper that allows one to learn partial systems with the `ADTLearner`.

For details, see the release notes of [LearnLib](https://github.com/LearnLib/learnlib/releases/tag/learnlib-0.16.0) and [AutomataLib](https://github.com/LearnLib/automatalib/releases/tag/automatalib-0.10.0).
