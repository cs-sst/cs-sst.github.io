---
layout: page
title : Talks by Hans de Nivelle
permalink : /faculty/nivelle/talks/index.md


## 2017 

<h3> Solving Satisfiability </h3>

Talk at ZOSIA 2017 (Przesieka)
<a href = "sat.pdf">Slides</a>.
<p>

The following problem is well-known to be NP-hard:
"Given a set of propositional clauses C, find an interpretation
that makes all clasues in C true".
Despite its NP-hardness, modern implementations are able to
solve large instances in short time. Other search problems
can be solved efficiently by translation them to SAT.
I explain the modern approach to SAT-solving, and demonstrate
use of <a href = "http://minisat.se/">MiniSat</a>.
Because of its fundamental nature, and the fact that
there exist efficient implementations, I think that
SAT-solving should be part of the standard curriculum.

## 2013 

<h3> Theorem Proving in Logic with Partial Functions </h3>

Talk at ZJP (Group of Programming Languages) in Wroclaw
<a href = "pcl_atp.pdf">Slides</a>, 
<a href = "pcl_atp_abstract">abstract</a>. 

## 2010 

<h3> Extending Classical Logic with Partial Functions </h3>

Talk was at the Kurt Goedel Colloquium, Technical University
of Vienna on 10.03.2010.

We give a natural semantics for classical logic
with partial functions (PCL).
The semantics is based on multi-valued logic, so that
formulas involving undefined values can have undefined
truth values. An unusual aspect of our semantics is that
it relies on the order of the formulas in a theory. 
The semantics is able to capture the fact that
functions and predicates must be declared before they are used.

We think that our approach to partial functions is more
natural than existing approaches, because in our approach,
formulas involving undefined values are guaranteed to be
undefined. In this way, PCL has the same strictness of simple
type theory, while at the same time being much more expressive.
<p>

(<a href = "wien2010slides.pdf">Slides</a>)


## 2007 

<h3> A study of Landau's Grundlagen der Analysis and AUTOMATH </h3>

In his Grundlagen der Analysis, Edmund Landau proves the basic 
properties of +.-.*,/ on the natural numbers, rational numbers, the
reals and the complex numbers from the Peano axioms. <p> 

In his introduction of addition and multiplication, there is a strange thing:
Both are introdued without reference to the fact that Nat is a free
data type. Especially the introduction of multiplication is a mystery. 
In order to check the proofs, we first give a precise description of 
Landau's introduction of addition and multiplication. After
this, the proof appears correct to us. <p> 

In 1977, the complete Grundlagen have been verified in the Automath system.
So we want to know: What is the mechanism used in Automath for 
introducting recursive functions, maybe Van Benthem Jutting used some kind of
additional recursion axiom for introducing addition and multiplication?
<p> 

We look into the sources of Van Benthem Jutting's translation, and 
see that the translation follows Landau's proof very carefully and
that no additional properties were used. <p>

So the question remains: How did Landau/Kalmar manage to get away without
using the fact that natural numbers are freely generated? Are
there more functions definable in that way? 

<p>

<a href = "grundlagenautomath2007/grundaut.ps"> ps </a> or
<a href = "grundlagenautomath2007/grundaut.pdf"> pdf </a>.


## 2006 

<h3> Geometric Resolution: A proof Procedure Based on Finite Model
     Search (Talk at Australian National University, November 2006) </h3>

The talk is essentially equal to the talk at IJCAR, but it contains
more details.

<a href = "canberra2006_slides.ps"> ps </a> or
<a href = "canberra2006_slides.pdf"> pdf </a>.


## Geometric Resolution: A Proof Procedure Based on Finite Model 
   Search (Talk at IJCAR 2006) </h3>

In the talk, I present a new calculus for first-order logic with
equality, which is called geometric resolution. The name derives
from the fact that the calculus operates on a normal form which
is remotely related to geometric logic, which was introduced by
Thoralf Skolem. 
We show that the calculus is refutationally complete for first-order logic.
A special feature of the calculus is that before proof search,
all function symbols are replaced by relations. 
Proof search operates by learning lemmas from failed model construction
attempts.
The calculus is implemented in geo, which got the best newcomer award
at the CASC competition.

<a href = "seattle2006_slides.ps"> ps </a> or
<a href = "seattle2006_slides.pdf"> pdf </a>.

## 2004 

<h3> Deciding Modal Logics through Relational Translations into GF2 </h3>

This is an extension of the talk with the same title from 2003.
We present ways of translating modal logics, that appear not to
be in the guarded fragment, into the guarded fragment by optimizing
the relational translation.
The translation works by expressing reachability properties
by regular automata, which can be translated into the guarded fragment.
We attempt to characterize for which modal logics such an
automaton can be constructed.
Download 
<a href = "nancy2004_slides.ps"> ps </a> or
<a href = "nancy2004_slides.pdf"> pdf </a>.

<h3> Translation of Resolution Proofs into Short First-Order Axioms
     without Choice Axioms </h3>

Talk given in Vienna. This is an improved version of the 
talk with the same title below. 
   <a href = "wien2004_slides.ps"> ps </a> or
   <a href = "wien2004_slides.pdf"> pdf </a>. 

## 2003

<h3> Translation of Resolution Proofs into Short First-Order Axioms
     without Choice Axioms </h3>

Talk was given in Dagstuhl, april 2003. 

   <a href = "dagstuhl2003_slides.ps"> ps </a> or
   <a href = "dagstuhl2003_slides.pdf"> pdf </a>.
   (The slides above, in 2004, are better) 

## 2002 

<h3> On the generation of Proofs from the Clausal 
     Normal Form Transformation </h3>

The talk was given at CSL 2002 in Edingburgh, Scotland.
   <a href = "csl2002_slides.ps"> ps </a> or
   <a href = "csl2002_slides.pdf"> pdf </a>.




