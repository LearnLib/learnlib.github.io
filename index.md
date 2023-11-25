---
layout: default
title: "LearnLib"
sidebar: learnlib
navbar-group: "Projects"
---

## Learnlib

LearnLib is a free and open source ([Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)) Java framework for automata learning.
It is mainly being developed at the [Chair of Programming Systems](http://ls5-www.cs.tu-dortmund.de/) at [TU Dortmund University, Germany](http://www.tu-dortmund.de/).
20 years of research in the field of automated learning as well as our experience in engineering software have gone into the development of LearnLib.

## Usage

In order to start using the latest, stable release of LearnLib in your **Maven** project, include the following snippet into the _dependencies_ section of the _pom.xml_.

```xml
<dependencies>
  <!-- other dependencies -->
  <dependency>
    <groupId>de.learnlib.distribution</groupId>
    <artifactId>learnlib-distribution</artifactId>
    <version>0.17.0</version>
    <type>pom</type>
  </dependency>
</dependencies>
```

_Note: This dependency will add all components of LearnLib to your project.
If you only need a subset, have a look at the [List of LearnLib Artifacts](https://github.com/LearnLib/learnlib/wiki/List-of-LearnLib-Artifacts) to get an overview of the individual modules available on **[Maven Central](http://mvnrepository.com/artifact/de.learnlib)**._

If you are not using any build management, you can also download the [distribution artifacts](https://central.sonatype.com/search?q=g:de.learnlib.distribution/) of LearnLib, with and without its dependencies.

[Examples](https://github.com/LearnLib/learnlib/tree/develop/examples/src/main/java/de/learnlib/example){: .btn .btn-sm .btn-outline-primary}
[Wiki](https://github.com/LearnLib/learnlib/wiki){: .btn .btn-sm .btn-outline-primary}
[API docs](http://learnlib.github.io/learnlib/maven-site/latest/apidocs/){: .btn .btn-sm .btn-outline-primary}

## Features

LearnLib provides a sophisticated set of active and passive learning algorithms for various automaton models as well as a variety of equivalence approximation strategies. Its modular, generic and extensible nature allows you to instantiate learning experiments that are tailored specifically to your needs. See the figure and the listing below to get a quick overview over all relevant features.

{% include features.html %}



#### Learning algorithms

| Algorithm (active)  | Target models               |     | Algorithm (passive) | Models                |
|---------------------|-----------------------------|-----|---------------------|-----------------------|
| AAAR                | `DFA` `Mealy` `Moore`       |     | OSTIA               | `SST`                 |
| ADT                 | `Mealy`                     |     | RPNI                | `DFA` `Mealy` `Moore` |
| DHC                 | `Mealy`                     |     | RPNI (EDSM)         | `DFA`                 |
| Kearns & Vazirani   | `DFA` `Mealy`               |     | RPNI (MDL)          | `DFA`                 |
| L* (incl. variants) | `DFA` `Mealy` `Moore`       |     |                     |                       |
| NL*                 | `NFA`                       |     |                     |                       |
| Observation Pack    | `DFA` `Mealy` `Moore` `VPA` |     |                     |                       |
| OML                 | `DFA` `Mealy`               |     |                     |                       |
| Procedural          | `SPA` `SBA` `SPMM`          |     |                     |                       |
| TTT                 | `DFA` `Mealy` `Moore` `VPA` |     |                     |                       |

#### Equivalence approximation strategies

- Complete, depth-bounded exploration
- Random words
- Random walk
- W-method
- W-method, randomised
- Wp-method
- Wp-method, randomised

#### More features

- Query cache
- Reuse filter
- Abstract to concrete system mapping
- Generic, extensible design
- Logging subsystem
