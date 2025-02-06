---
layout: default
title: "LearnLib"
sidebar: learnlib
navbar-group: "Projects"
---

## LearnLib

LearnLib is a free and open-source ([Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)) Java framework for automata learning.
It is mainly being developed at [TU Dortmund University, Germany](https://cs.tu-dortmund.de/).
20 years of research in the field of automated learning as well as our experience in engineering software have gone into the development of LearnLib.

## Usage

In order to start using the latest, stable release of LearnLib in your **Maven** project, include the following snippet into the _dependencies_ section of the _pom.xml_.

```xml
<dependencies>
  <!-- other dependencies -->
  <dependency>
    <groupId>de.learnlib.distribution</groupId>
    <artifactId>learnlib-distribution</artifactId>
    <version>0.18.0</version>
    <type>pom</type>
  </dependency>
</dependencies>
```

_Note: This dependency will add all components of LearnLib to your project.
If you only need a subset, have a look at LearnLib's [modules](https://learnlib.github.io/learnlib/maven-site/latest/apidocs/) which correspond to the individual artifacts available on **[Maven Central](http://mvnrepository.com/artifact/de.learnlib)**._

If you are not using any build management, you can also download the [distribution artifacts](https://central.sonatype.com/search?q=g:de.learnlib.distribution/) of LearnLib, with and without its dependencies.

[Examples](https://github.com/LearnLib/learnlib/tree/develop/examples/src/main/java/de/learnlib/example){: .btn .btn-sm .btn-outline-primary}
[Wiki](https://github.com/LearnLib/learnlib/wiki){: .btn .btn-sm .btn-outline-primary}
[API docs](http://learnlib.github.io/learnlib/maven-site/latest/apidocs/){: .btn .btn-sm .btn-outline-primary}

## Features

LearnLib provides a sophisticated set of active and passive learning algorithms for various automaton models as well as a variety of equivalence approximation strategies. Its modular, generic and extensible nature allows you to instantiate learning experiments that are tailored specifically to your needs. See the figure and the listing below to get a quick overview over all relevant features.

{% include features.html %}



#### Learning algorithms

| Algorithm (active)  | Target models               |     | Algorithm (passive)   | Models                |
|---------------------|-----------------------------|-----|-----------------------|-----------------------|
| AAAR                | `DFA` `Mealy` `Moore`       |     | OSTIA                 | `SST`                 |
| ADT                 | `Mealy`                     |     | RPNI (incl. variants) | `DFA` `Mealy` `Moore` |
| DHC                 | `Mealy`                     |     |                       |                       |
| Kearns & Vazirani   | `DFA` `Mealy`               |     |                       |                       |
| Lambda              | `DFA` `Mealy`               |     |                       |                       |
| L#                  | `Mealy`                     |     |                       |                       |
| L* (incl. variants) | `DFA` `Mealy` `Moore`       |     |                       |                       |
| NL*                 | `NFA`                       |     |                       |                       |
| Observation Pack    | `DFA` `Mealy` `Moore` `VPA` |     |                       |                       |
| Procedural          | `SPA` `SBA` `SPMM`          |     |                       |                       |
| TTT                 | `DFA` `Mealy` `Moore` `VPA` |     |                       |                       |

#### Equivalence approximation strategies

- Complete, depth-bounded exploration
- Random words
- Random walk
- (partial) W-method (incl. variants)
- Black-Box Checking (via [LTSmin](https://ltsmin.utwente.nl/))

#### More features

- Query cache
- Parallel oracles
- Statistics
- Reuse filter
- Abstract to concrete symbol mapping
- Generic, extensible design
