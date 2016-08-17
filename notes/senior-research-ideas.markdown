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
system in its entirety? Or at least a large subset of git that is
commonly encountered in daily use?

If such a system could be built, then it would be able to suggest a
series of actions to fix most git messes. It could be used by individuals
to assist in their daily software development. It could also be used
during automated deployments to ensure the repository is in a certain
state. In short, many developers around the world would be very
interested if such a system existed. Significant internet points can
be had.

### Student advisor

The
[fifth assignment in my AI class](http://csci431.artifice.cc/assignments/a05.html)
asks students to build a system that advises computer science students at
Stetson in their course selection. The idea is that the system would take the
place of a faculty adviser, at least for relatively straightforward advising
scenarios. The system would be built with a set of rules that mirror the
University rules for coursework and the kinds of thought processes a human
advisor would entertain depending on the student's particular situation. The
result would be like a smarter Degree Audit tool that guided students like an
advisor would.

A more extensive version of this system would automate more aspects of the
advising relationship, such as scheduling of summer courses, consideration of
minors, support for more majors, general education requirements, etc. A domain
specific language can be designed to allow advising experts but non-computer
programmers to validate and possibly update the knowledge base. Furthermore,
the system could present a user interface in which the software acts as an
assistant for faculty advisors across campus.

### Pentesting/intrusion/exploitation plan recognition

Suppose Dr. Plante is teaching the computer security course and each student has his/her own virtual machine on the delenn server. Each student is attempting to find vulnerabilities in the VM's services. Suppose further that Dr. Plante is able to monitor and record all network traffic to/from each student's VM. Is it possible to recognize the kinds of pentesting or intrusions or exploitation techniques that the student is using? Can we understand how students find successful vulnerabilities or identify reasons they fail to do so? With such a recognition engine, we could build an automated tutoring system that guides students on the right path.

Some existing research exists for (separately) intrusion detection from network traffic signatures and plan recognition. By combining the two subfields of AI and computer security, we could produce a useful tool for computer security educators.

See the project idea below, "Automated configuration of computer security scenarios," for a companion project.

### American Sign Language tutor

Is it possible to build a computer-based sign language recognition
system that uses only a computer or smartphone's built-in camera? This
project was the subject of earlier senior research. The next task in
this project is to find a way to use deep learning or another technique to
train an accurate recognizer using a set of training images. Assuming that
works, a usable application could be built and possibly fashioned into a
computer-based tutoring system for ASL learners. Current ASL tutoring systems
require special gloves or other sensors.  The benefit with the proposed system
is that it would be low-cost and usable by anyone with a laptop or smartphone,
though this constraint brings significant challenges in accurately recognizing
signs.


### Recommendations based on contextual proximity

This idea was contributed by Jeffrey Wray of Mobilozophy (jwray@mobilozophy.com), CSCI alumnus from 2009. Using a grid of inexpensive Bluetooth LE beacons in a large space, can we identify and analyze the travel paths and other behaviors of people and make individualized recommendations? E.g., can we recommend products and services to customers wandering around a store or public market? Can we build an individualized tour guide for visitors in a museum by inferring their interests based on the exhibits they visit? Can we optimize a space for efficient crowd flow by detecting choke points and idling? This project combines several aspects of AI such as sensor-based tracking, behavior recognition, and recommendation engines.

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

## Computing infrastructure

### Automated configuration of computer security scenarios

The computer security course at Stetson, and others like it at many colleges, was designed by Dr. Plante to give students realistic scenarios for penetration testing, exploitation and exploit detection, etc. He and I have begun working on a declarative language for defining scenarios and corresponding tool that generates a host of virtual machines (e.g., one VM per student or group) with specific operating system, network, and application configurations. The configurations are determined by the predefined textual scenarios. Vagrant and Ansible are used to launch and configure the VMs.

According to my research, no such tool exists. There are various repositories of prebuilt VM images for various security course scenarios. What we hope to offer is a more flexible tool in which the scenarios are defined in a text file, and the VM images are built on-demand. With this flexibility, the scenarios could even be randomly generated (for exam situations). They can also be shared among the community of security educators as the scenarios will be defined by simple text files rather than shared as complete VM images.

We already have a start on the implementation. See [this GitHub repository](https://github.com/StetsonMathCS/openvsec).

## Other ideas

Please talk to me if you have other ideas. Consider using some of the
following devices previously purchased for senior research:

- Fitbit Surge (fitness/health monitoring)
- iPod Touch (mobile apps)
- Kinect (interfaces, games)
- Muse headband (brainwave monitoring)
- 4-wheeled robot with arm gripper, two cameras, LIDAR (robotics)

The Math/CS department typically purchases more equipment upon request.

