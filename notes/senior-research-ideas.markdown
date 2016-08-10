---
title: Senior research ideas
layout: note
---

# Senior research ideas

If you are looking for a senior research project, consider the
following ideas, or talk to me to brainstorm new ones.

## Artificial intelligence

### Git planner

The
[second assignment in my AI class](http://csci431.artifice.cc/assignments/a02.html)
asks students to build a system that generates a series of git
commands to transform a repository from some starting state to some
goal state. In other words, it finds a plan for you to get out of a
"git mess."

The assignment is limited to a single repository with no
branches. However, realistic git messes involve merge conflicts and
pull/push operations and cherry-picking and stashes and so on... Is it
possible to build a planning knowledge base that represents the git
system in its entirety? Or at least a large part of git that is
commonly encountered in daily use?

If such a system could be built, then it would be able to suggest a
series of actions to fix any git mess. It could be used by individuals
to assist their daily software development. It could also be used
during automated deployments to ensure the repository is in a certain
state. In short, many developers around the world would be very
interested if such a system existed. Significant internet points can
be had.

### Student advisor

The
[fifth assignment in my AI class](http://csci431.artifice.cc/assignments/a05.html)
asks students to build a system that advises computer science students
at Stetson in their course selection. The idea is that the system
would take the place of a faculty adviser, at least for relatively
straightforward advising scenarios. The system would be built with a
set of rules that mirror the kinds of thought processes a human
advisor would entertain depending on the student's particular
situation.

A more extensive version of this system would automate more aspects of
the advising relationship, such as scheduling of summer courses,
consideration of minors, support for more majors, etc. Ultimately, the
system could expose a user interface in which the software acts as an
assistant for faculty advisors across campus.

### American Sign Language tutor

Is it possible to build a computer-based sign language recognition
system that uses only a computer or smartphone's built-in camera? This
project was the subject of earlier senior research. The next task in
this project is to find a way to use deep learning or another
technique to train an accurate recognizer using a set of training
images. Assuming that works, a usable application should be built and
possibly fashioned into a computer-based tutoring system for ASL
learners. Current ASL tutoring systems are very limited or require
special gloves or other sensors. The benefit with the proposed system
is that it would be low-cost and usable by anyone with a laptop or
smartphone, though this constraint brings significant challenges in
accurately recognizing signs.

## Programming languages

### Spoken programming language

Is it possible to design a useful programming language that can be
spoken and heard? What kind of "syntax" would be appropriate? How can
we keep the semantics constrained so that a programmer's short term
working memory is not overloaded with deeply nested logic or long
functions or too many functions? Which programming paradigms
(procedural, functional, logical, object-oriented, etc.) are most
appropriate for "programming in your head"? How can we implement a
speech recognition system that is sufficiently accurate for this task?

Any successful work in this project is surely publishable, since
nothing like it exists. The closest work that I have found is speech
recognition for programming Java (i.e., speaking Java code). A spoken
programming language, on the other hand, may need to be unlike any
other programming language since the code cannot be seen. All
programming would have to be mental, so limits to short term working
memory become very important.

### Visual homoiconic programming language

Homoiconic languages are those in which the code is written in the
same way as data, so code can be processed as data. One benefit of
homoiconic languages is that code can be generated or transformed
during compilation or execution. Examples of homoiconic languages are
the various Lisp languages, Prolog, and Tcl.

Unrelated to homoiconic languages, visual languages allow programmers
to write "code" with visual constructs instead of text. These
constructs may take the form of colored shapes representing abstract
art, as with the Piet language, or data flow models like Max.

To my knowledge, there is no language that is both homoiconic and
visual. Is that even possible? What visual construct would represent a
function or unit of execution? A square perhaps? That representation
should also work for data as well as code, i.e., a square could also
be input to a function (so, squares consume squares). The payoff of
such a project is that you would develop something completely
novel. Bonus points if it can also be made useful.

## Other ideas

Please talk to me if you have other ideas. Consider using some of the
following devices previously purchased for senior research:

- Fitbit Surge (fitness/health monitoring)
- iPod Touch (mobile apps)
- Kinect (interfaces, games)
- Muse headband (brainwave monitoring)
- 4-wheeled robot with arm gripper, two cameras, LIDAR (robotics)

The Math/CS department typically purchases more equipment upon request.

