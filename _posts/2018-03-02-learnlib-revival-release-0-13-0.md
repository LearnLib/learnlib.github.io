---
layout: post
title: "LearnLib revival - Release 0.13.0"
date: "2018-03-02"
navbar-group: "News"
author: "Markus Frohme"
categories:
  - "pages"
  - "news"
---

Good things are worth waiting for!

After a nearly 2 year hiatus due to the departure of the core research assistants behind the project, development of the LearnLib and AutomataLib has been picked up again mid 2017.
We are happy to announce that these efforts have culminated in new releases for both [LearnLib](https://github.com/LearnLib/learnlib/releases/tag/learnlib-0.13.0) and [AutomataLib](https://github.com/LearnLib/automatalib/releases/tag/automatalib-0.7.0), early this February.

Most notably, the new releases added support for learning visibly push-down automata, added a new active learning algorithm utilizing adaptive distinguishing sequences and added initial support for passive automata learning in the form of three passive learning algorithms.
Furthermore, the learning process itself has been enhanced by allowing to dynamically increase hypothesis alphabets during the learning process and suspending/resuming learners for improved managing of the learning process.

On the code side, we have cleaned up the project structure to allow you to pick exactly the components you need for your application.
We refurbished the build ecosystem and set up continuous integration and continuous deployment services, that pave the way for future development and cooperation.
To get your hands on the code, head over to the GitHub pages of [LearnLib](https://github.com/LearnLib/learnlib) and [AutomataLib](https://github.com/LearnLib/automatalib).

Let's make automata learning great again.
