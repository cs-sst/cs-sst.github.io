---
layout: page
title: Software
permalink: /faculty/nivelle/software/index.md
---

## Geo III

At this moment, Geo III is an unfinished prover for classical logic 
with partial functions, based on 
<a href = "http://www.ii.uni.wroc.pl/~nivelle/publications/jlc2014.pdf">
Kleene logic</a>.
In the current version, only Chapters 4 and 5 have been implemented,
and the transformation from first-order logic to geometric logic
is still 2-valued. 
The goal of Geo III is to implement the complete logic.
I assume that this goal will be reached in the fall of 2015,
because I implemented the hardest part first. 

### Downloading

<ul>
<li>
   The latest version is geo2015E.
   It can be downloaded from 
   <a href = "http://www.cs.miami.edu/~tptp/CASC/25/SystemsSources/">CASC</a>.
   Note that Geo is released under GNU General Public Licence, Version 3.
</li>
</ul>

### Running Geo

In order to run geo, unzip and untar. If you are lucky, you
type './geo < blz202_4.geo' and you see that geo finds a proof.

Otherwise, type  'touch Makefile', type 'make' and hope that
the resulting executable works. You need a reasonably
new version of g++, because Geo uses C++11.

Geo accepts the following parameters:
<dl>
<dt> -inputfile %f. 
<dd> Instead of reading from standard input, read from the
   indicated file %f.
<dt> -nonempty. 
<dd> Do not allow empty models. Without this flag, geo cannot prove
    forall x. p(x) -> exists x. p(x), because the empty model
    is a counter model.
<dt> -tptp_input. 
<dd> Expect input in TPTP-format. 
<dt> -include %p
<dd> Use %p as the path, relative to which include files are defined.
    TPTP-syntax allows includes. 
</dl>


## Matching, Constraint Solver 
Because geometric resolution relies heavily on constraint solving,
the constraint solver is currently the most sophisticated part of Geo.
The implementation is probably efficient enough for independent use,
outside of geometric resolution. Therefore, we publish the constraint
solver as standalone package. The implementation is in portable C++(11).
Solver reads input from stdin, and prints outpout into stdout. 
The input format is similar
to DIMACS format for first-order logic, it is described in Section 7 of 
<a href = "GCSP.pdf">this article</a>, which also describes the matching
algorithm.  

<a href = "solver.tar.gz">These</a> are the sources.

There are different benchmark sets.




