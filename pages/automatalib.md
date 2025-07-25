---
layout: default
title: "AutomataLib"
description: "An open library for modeling automata, graphs, and transition systems"
image: "/assets/images/automatalib.svg"
sidebar: automatalib
navbar-group: "Projects"
---

## AutomataLib

AutomataLib supports modeling a variety of graph-based structures.
Currently, it covers generic transition systems, Deterministic Finite Automata (DFA) and Mealy machines as well as more advanced structures such as Visibly Pushdown Automata (VPAs) and procedural systems (SPAs, SBAs, SPMMs).

Models of AutomataLib can be (de-)serialized (from) to one of the various supported serialization formats and may be visualized using either the GraphViz or JUNG library.
Furthermore, a plethora of graph-/automata-based algorithms is implemented, covering the following topics:

- graph theory (traversal, shortest paths, strongly-connected components)
- automata theory (bisimulation, equivalence, minimization)
- model checking (adaptive distinguishing sequences, (partial) W-method, characterizing sets, state/transition covers, LTL checking (via [LTSmin](https://ltsmin.utwente.nl/) and M3C)

## Usage

In order to start using the latest, stable release of AutomataLib in your **Maven** project, include the following snippet into the _dependecies_ section of the _pom.xml_.

```xml
<dependencies>
  <!-- other dependencies -->
  <dependency>
    <groupId>net.automatalib.distribution</groupId>
    <artifactId>automata-distribution</artifactId>
    <version>0.12.0</version>
    <type>pom</type>
  </dependency>
</dependencies>
```

_Note: This dependency will add all components of AutomataLib to your project. If you only need a subset, have a look at AutomataLib's [modules](https://learnlib.github.io/automatalib/maven-site/latest/apidocs/) which correspond to the individual artifacts available on **[Maven Central](http://mvnrepository.com/artifact/net.automatalib)**._

If you are not using any build management, you can also [download the binaries](http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22net.automatalib.distribution%22) of AutomataLib, with and without its dependencies.

[Examples](https://github.com/LearnLib/automatalib/tree/develop/examples/src/main/java/net/automatalib/example){: .btn .btn-sm .btn-outline-primary}
[Wiki](https://github.com/LearnLib/automatalib/wiki){: .btn .btn-sm .btn-outline-primary}
[API docs](http://learnlib.github.io/automatalib/maven-site/latest/apidocs/){: .btn .btn-sm .btn-outline-primary}
