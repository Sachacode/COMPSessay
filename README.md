# Software Foundations: Coq Tutorial

## Replication Instructions

There are several dependancies that need to be installed before Coq, all commands are for a Mac system because I work on Mac.

Install Homebrew
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Install Opam
```
brew install gpatch
brew install opam
```
Create switch for Coq enviornment
```
opam switch create coq-8.12.0 ocaml-base-compiler.4.11.0
```
Utop contains many important dependancies.
```
opam install utop
```
Install Coq
```
opam pin add coq 8.12.0
```
Check installation
```
coqtop
```

[Software Foundations Source Files](https://softwarefoundations.cis.upenn.edu/lf-current/index.html)

[Install VSCode](https://code.visualstudio.com/)

[Install Coq plugin](https://marketplace.visualstudio.com/items?itemName=maximedenes.vscoq)

## Code Architecture Overview

A large number of files have been provided, the only important ones are the files for the first three chapters: Basics.v, Induction.v, and Lists.v are the only relevant files that I worked through. Each file is like a chapter from a textbook. Information is given with comments and provided functions, theorems, and proofs, these are not sections that I wrote and are from the textbook. All of the work I did is found on sections labeled exercise in comments. The difficulty of exercises varies with the number of stars.
- one stars are easy, time estimated 1-2 minutes
- two stars are standard, time estimated for 5-10 minutes
- three stars are hard, time estimated for 10-30 minutes
- four/five stars are extreme, time estimated for 30+ minutes

Run `make` in the terminal to save all defined functions, theorems, and proofs.
```
make
```

When checking a proof, press control + alt + down arrow to run a part of the proof. Press control + alt + up arrow to un-run any section of code. Press control + alt + right arrow to jump ahead or behind to wherever the cursor is.

To run my solutions, simply download the files for the Software Foundations, then replace the files with the ones provided.

