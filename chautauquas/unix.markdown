---
title: Unix
layout: note
---

# Unix

show Cathode “Space Opera” favorite before starting

quarter century of unix: salus1994quarter

## Outline

??? what computing systems are in use today?
- android
- ios
- mac os x
- windows
- linux

all but windows are direct descendants of Unix; windows has been influenced by Unix but is not a direct descendant.

## What is Unix used for? Why is it useful?

- normal desktop machines
	- Ubuntu
	- Linux Mint
	- Mac OS X
- supercomputers
	- [top500 list](http://www.top500.org/statistics/list/)
- watches
	- WatchOS (Apple Watch)
	- Android (Samsung Galaxy Gear, etc.)
- phones, tablets
	- Android
	- iOS
- gaming consoles (soon?)
	- Steam Machine
- big data processing, cloud services
	- from Amazon, Microsoft, Google, Digital Ocean, etc.
- mainframes
	- IBM z/OS Unix System Services
- Windows 7+
	- Cygwin

What’s it good for?
- everything?
- school work, CS research
- automation
- hacking
- customization (unix porn)
- elitism

But not good for:
- many games (e.g., Skyrim, The Witcher 3, etc.)
- some important applications:
	- Adobe Photoshop, et al. (Creative Suite)
	- Logic Pro
	- Microsoft Office

## Origin of Unix

[Unix History timeline](http://www.levenez.com/unix/)

**Use Cathode for examples**

Timesharing:

- better than batch processing!
- early ideas by John McCarthy
- first deployment 1962
- standard terminal: ASR-33 (show image)
	- terse commands were appreciated!

CTSS: Compatible Timesharing System
- 1961 - 1973
- “compatible” because it was able to run batch jobs for FORTRAN

Multics: Multiplexed Information Computing Service

- 1964 - 2000
- second generation timesharing system
- Ken Thompson worked on the project
- goals:
	- convenient remote terminal use
	- continuous operation (like telephone service)
	- hierarchical structures of data
	- support wide range of applications
	- etc.
- suffered from second-system effect:
	- supposed to do all things, be perfect
	- became increasing complex
	- Unix born from Bell Labs exiting Multics project

Contribution of Multics:

- tree-structured file system
- separate “shell” program (even name taken from Multics)
	- just a user process; not a kernel command interpreter!
- files have no internal structure; just bytes
- text files are just sequence of characters with newlines
- input/output is just bytes in/out without worrying about disk blocks, etc.

Unix:

- Dennis Ritchie, Ken Thompson, others at Bell Labs
- began on PDP-7 (relatively cheap machine)
- started on file system design; devices as “files”; then added processes to make use of the file system
- name: “it was not until well into 1970 that Brian Kernighan suggested the name ‘Unix,’ in a somewhat treacherous pun on ‘Multics’” ([source](https://www.bell-labs.com/usr/dmr/www/hist.html))
	- originally: UNICS (“UNiplexed Information and Computing Service”)
- upgraded to PDP-11:
	- proposed purchase of PDP-11 to support word processing
	- they added some features to `roff` to beat another competing system on Multics
		- for Bell Labs’ patent department
	- hence, introduction of various word processing utilities
	- used by secretaries
- early uses on weak machines
	- **”constraint has encouraged not only economy, but also a certain elegance of design”**
- C language (from Ritchie):
	- they ported interpreters for BCPL and B (latter simplified version of former)
	- C added types, structs
	- eventually, Unix kernel rewritten in C
- Unix easily ported to other machines
- deployment increased at universities, corporations, government
	- often on weaker machines
	- more people could use it (on weaker machine), created a culture (counterculture), lots of ideas
- Berkeley center of a lot of activity
	- BSD Unix
	- TCP/IP
	- vi
- GNU (1985)
	- never finished kernel
- Linux: Sun machines too expensive, wanted a good Unix for i386; BSD386 not released until after Torvalds started his project
	- used GNU tools (compiler, bash, etc.)
	- Torvalds has stated, "making Linux GPL'd was definitely the best thing I ever did."

“The Linux and BSD development efforts were native to the Internet in a way previous Unixes had not been. They relied on distributed development and Larry Wall's patch(1) tool, and recruited developers via email and through Usenet newsgroups.” ([source](http://www.catb.org/esr/writings/taoup/html/ch02s01.html))

## UI paradigm

Compare TOPS-20:
- 1976 - 1988
- for PDP-10 (not -7 or -11), totally different machine (bigger, mainframe machine; -7 and -11 are minicomputers; a minicomputer like the -11 would be used to boot a -10)

TOPS-20: command line assistance

- resume Rhizome
- completion/help examples:
	- dir
	- pwd
	- dir ?
	- dir sys:?
	- dir sys:ud$
	- help ?
	- help pdp-8 (interactive help contents)
	- help jargon

Early Unix: obscure, no assistance

[Unix Hater’s Handbook](http://web.mit.edu/simsong/www/ugh.pdf)

## Unix philosophy

> (i) Make each program do one thing well. To do a new job, build afresh rather than complicate old programs by adding new features.
> (ii) Expect the output of every program to become the input to another, as yet unknown, program. Don't clutter output with extraneous information. Avoid stringently columnar or binary input formats. Don't insist on interactive input.
> (iii) Design and build software, even operating systems, to be tried early, ideally within weeks. Don't hesitate to throw away the clumsy parts and rebuild them.
> (iv) Use tools in preference to unskilled help to lighten a programming task, even if you have to detour to build the tools and expect to throw some of them out after you've finished using them.
> ([source](http://www.catb.org/esr/writings/taoup/html/ch01s06.html))

Unix philosophy not always met:

- `ls -S` (sort by file size) vs. `ls | sort`
- `man cat` on Mac OS X:
	- see also: UNIX Style, or cat -v Considered Harmful
		- `cat -v` shows non-printable characters as ASCII
		- confuses concatenating files (for whatever purpose) with showing files on the terminal

## Unix file system hierarchy

Londo: (just walk through it)

	man hier

## Basic commands

Note in UnixV6, lines scroll off screen; no `more` or `less` or `pg` command. Expected hard-copy ttys. Glass ttys started appearing in wide usage in the late 70’s, early 80’s. `more` command invented in 1978. Unix V6 released in 1975.

### ed

	ed
	e /etc/passwd (open for editing)
	f (print current filename)
	g/3/p (run ‘p’ (print) command on all lines matching regex 3)
	v/3/p (run ‘p’ on all lines not matching regex 3)
	i (insert before)
	a (append after)
	c (change current line to something else)
	1,$p (print whole file)
	= (show current line number)
	3 (followed by enter; shows that line)
	(blank; followed by enter: equivalent to .+1p)
	s/josh/james/g
	$s/josh/james/g
	1,3s/josh/james/ (supports \1 substitutions as well)
	1,3m5 (move lines 1-3 after line 5)
	w (write)
	q (quit)

[ed is the standard text editor](http://www.gnu.org/fun/jokes/ed-msg.txt)

Expanded to `ex` later by Bill Joy, who also created `vi` (“visual”) at the same time (for visual editing). vi takes most ex commands at the `:` prompt.

### banner

	banner acm club

## Modern Unix tools

	man
	apropos

bash features (for loops, etc. - show man page)

Londo:

	cd ~/acmclub/unix
	./mp3info-0.8.5a/mp3info -p "%S\n" mp3files/nine_inch_nails_the_slip/...
	for ...

sum up numbers: 

	(prior command) | paste -s -d+ | bc # -s for serial, -d for delimiter

	units -t '360 seconds' 'minutes' # (-t for terse)


## Linux distributions

Count: [DistroWatch Weekly](http://distrowatch.com/weekly.php?issue=20160125), see bottom:

> Number of all distributions in the database: 805
> Number of active distributions in the database: 273
> Number of dormant distributions: 64
> Number of discontinued distributions: 468
> Number of distributions on the waiting list: 257

Go to some random distros (button at top). (Some BSDs, other OS’s are included on that site.)

Later ACM event: Linux InstallFest

## Get your own Unix

- Ubuntu, Linux Mint, etc.
- Mac OS X
- Campus accounts: delenn, londo
- SDF
- LivingComputerMuseum.org
