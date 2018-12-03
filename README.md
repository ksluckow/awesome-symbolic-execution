# Awesome Symbolic Execution [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

>A curated list of awesome symbolic execution resources including essential research papers, lectures, videos, and tools.


## Table of Contents

* [Papers](#papers)
* [Courses](#courses)
* [Videos](#videos)
* [Tools](#tools)


## Papers

* [Symbolic Execution and Program Testing](https://doi.org/10.1145/360248.360252), James C. King.
* [A system to generate test data and symbolically execute programs](https://doi.org/10.1109/TSE.1976.233817), L. A. Clarke.
* [All You Ever Wanted to Know about Dynamic Taint Analysis and Forward Symbolic Execution (but Might Have Been Afraid to Ask)](https://doi.org/10.1109/SP.2010.26), Edward J. Schwartz, Thanassis Avgerinos, David Brumley.
* [A Survey of Symbolic Execution Techniques](https://arxiv.org/pdf/1610.00502.pdf), Roberto Baldoni, Emilio Coppa, Daniele Cono D’Elia, Camil Demetrescu, and Irene Finocchi.


## Courses

* [Symbolic Execution Lecture at Harvard](http://www.seas.harvard.edu/courses/cs252/2011sp/slides/Lec13-SymExec.pdf).
* [Symbolic Execution Lecture at Iowa State University](http://web.cs.iastate.edu/~weile/cs641/9.SymbolicExecution.pdf).
* [Symbolic Execution Lecture at University of Maryland](https://www.cs.umd.edu/class/spring2013/cmsc631/lectures/symbolic-exec.pdf).


## Videos

* [Symbolic Execution Lecture at MIT](https://www.youtube.com/watch?v=mffhPgsl8Ws).
* [Symbolic Execution Lecture (part of Software Security course on Coursera)](https://www.coursera.org/learn/software-security/lecture/agCNF/introducing-symbolic-execution).


## Tools


### Java

* [Symbolic PathFinder (SPF)](https://babelfish.arc.nasa.gov/trac/jpf/wiki/projects/jpf-symbc) - Symbolic execution tool built on [Java PathFinder](https://babelfish.arc.nasa.gov/trac/jpf/). Supports multiple constraint solvers, lazy initialization, etc.
* [JDart](https://github.com/psycopaths/jdart) - Dynamic symbolic execution tool built on [Java PathFinder](https://babelfish.arc.nasa.gov/trac/jpf/). Supports multiple constraint solvers using [JConstraints](https://github.com/psycopaths/jconstraints).
* [CATG](https://github.com/ksen007/janala2) - Concolic execution tool that uses [ASM](http://asm.ow2.org/) for instrumentation. Uses CVC4.
* [LimeTB](http://www.tcs.hut.fi/Software/lime/) - Concolic execution tool that uses [Soot](https://sable.github.io/soot/) for instrumentation. Supports [Yices](http://yices.csl.sri.com/) and [Boolector](http://fmv.jku.at/boolector/). Concolic execution can be distributed.
* [Acteve](https://code.google.com/archive/p/acteve/) - Concolic execution tool that uses [Soot](https://sable.github.io/soot/) for instrumentation. Originally for Android analysis. Supports [Z3](https://github.com/Z3Prover/z3).
* [jCUTE](http://osl.cs.illinois.edu/software/jcute/) - Concolic execution tool that uses [Soot](https://sable.github.io/soot/) for instrumentation. Supports [lp_solve](http://lpsolve.sourceforge.net/).
* [JFuzz](http://people.csail.mit.edu/akiezun/jfuzz/) - Concolic execution tool built on [Java PathFinder](https://babelfish.arc.nasa.gov/trac/jpf/).
* [JBSE](http://pietrobraione.github.io/jbse/) - Symbolic execution tool that uses a custom JVM. Supports CVC3, CVC4, Sicstus, and Z3.
* [Key](https://www.key-project.org/) - Theorem Prover that uses specifications written in Java Modeling Language (JML).


### LLVM

* [KLEE](http://klee.github.io/) - Symbolic execution engine built on LLVM.
* [Cloud9](http://cloud9.epfl.ch/) - Parallel symbolic execution engine built on KLEE.
* [Kite](http://www.cs.ubc.ca/labs/isd/Projects/Kite/) - Based on KLEE and LLVM.
* [SymCC](https://github.com/eurecom-s3/symcc) - A compiler wrapper which embeds symbolic execution into the program during compilation, and an associated run-time support library.

### .NET

* [PEX](http://pex4fun.com/About.aspx) - Dynamic symbolic execution tool for .NET.


### C

* [CREST](https://github.com/jburnim/crest).
* [Otter](https://bitbucket.org/khooyp/otter/).
* [CIVL](http://vsl.cis.udel.edu/civl/) - A framework that includes the CIVL-C programming language, a model checker and a symbolic execution tool.


### JavaScript

* [Jalangi2](https://github.com/Samsung/jalangi2).
* [SymJS](https://doi.org/10.1145/2635868.2635913).


### Python

* [CrossHair](https://github.com/pschanely/CrossHair) - Symbolic execution tool for verifying properties of Python functions.
* [PyExZ3](https://github.com/thomasjball/PyExZ3) - Symbolic execution of Python functions. A rewrite of the [NICE](https://code.google.com/archive/p/nice-of) project's symbolic execution tool.


### Ruby

* [Rubyx](https://www.cs.umd.edu/~avik/papers/ssarorwa.pdf) - Symbolic execution tool for Ruby on Rails web apps.


### Android

* [SymDroid](http://www.cs.umd.edu/~jfoster/papers/cs-tr-5022.pdf).


### Binaries

* [Mayhem](http://dx.doi.org/10.1109/SP.2012.31).
* [SAGE](https://patricegodefroid.github.io/public_psfiles/ndss2008.pdf) - Whitebox file fuzzing tool for X86 Windows applications.
* [DART](https://doi.org/10.1145/1064978.1065036). 
* [BitBlaze](http://bitblaze.cs.berkeley.edu/).
* [PathGrind](https://github.com/codelion/pathgrind) - Path-based dynamic analysis for 32-bit programs.
* [FuzzBALL](http://bitblaze.cs.berkeley.edu/fuzzball.html) - Symbolic execution tool built on the BitBlaze Vine component.
* [S2E](http://s2e.systems/) - Symbolic execution platform supporting x86, x86-64, or ARM software stacks.
* [miasm](https://github.com/cea-sec/miasm) - Reverse engineering framework. Includes symbolic execution.
* [pysymemu](https://github.com/feliam/pysymemu/) - Supports x86/x64 binaries.
* [BAP](https://github.com/BinaryAnalysisPlatform/bap) - Binary Analysis Platform provides a framework for writing program analysis tools.
* [angr](http://angr.io/) - Python framework for analyzing binaries. Includes a symbolic execution tool.
* [Triton](https://triton.quarkslab.com/) - Dynamic binary analysis platform that includes a dynamic symbolic execution tool.
* [manticore](https://github.com/trailofbits/manticore) - Symbolic execution tool for binaries (x86, x86_64 and ARMV7) and Ethereum smart contract bytecode.
* [BinCAT](https://github.com/airbus-seclab/bincat) - Binary code static analyser, with IDA integration. Performs value and taint analysis, type reconstruction, use-after-free and double-free detection.


### Misc

* [Symbooglix](https://github.com/symbooglix/symbooglix) - Symbolic execution tool for Boogie programs.
