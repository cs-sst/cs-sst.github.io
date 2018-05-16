---
layout: page
title: Publications
permalink: /faculty/nivelle/publications/index
---

# Publications 

## 2016 

### Subsumption Algorithms for Three-Valued Geometric Resolution 

In the implementation of geometric resolution, the
most costly operation is subsumption (or matching).
In the matching problem,
one has to decide for a three-valued, geometric formula,
whether this formula is false in a given interpretation.
The formula contains only atoms with variables, equality, and existential
quantifiers. The interpretation contains only atoms with constants,
which are assumed to be distinct. 

Because matching is not restricted by term structure,
matching for geometric resolution is a hard problem.
We translate the matching problem into a generalized constraint
satisfaction
problem, and give an algorithm that solves it efficiently.
The algorithm uses learning teachings, similar to clause learning
in propositional logic. After that, we adapt the algorithm in
such a way that it finds solutions that use a minimal subset of
the interpretation. 

The techniques presented in this paper may also have applications
in constraint solving. 

The paper was presented at [IJCAR](http://www.ijcar-2016.info).
A preprint is available [here](ijcar2016.pdf).
I also gave [a talk](zjp2016.pdf) about this at the local seminar
in Wroclaw.

## 2014? 

### Theorem Proving for Classical Logic with Partial Functions by Reduction to Kleene Logic 

Partial functions are abundant in mathematics and program
specifications. Despite this, their importance has been mostly ignored
in automated theorem proving.
In this paper, we develop a theorem proving strategy for
Partial Classical Logic (PCL).
Proof search takes place in Kleene Logic. We show that
PCL theories can be translated into equivalent sets of formulas
in Kleene logic. For proof search in 
Kleene logic, we use a three-valued adaptation of geometric
resolution. We prove that the procedure is sound and
complete. 

The paper has appeared in 
[Journal of Logic and Computation](http://logcom.oxfordjournals.org/),
and [this](jlc2014.pdf) is a preprint.

## 2011 

### Classical Logic with Partial Functions 

In this paper, I introduce a semantics for classical logic with partial
functions, in which ill-typed formulas are guaranteed to have
no truth value, so that they cannot be used in any form of reasoning.
The semantics makes it possible to mix reasoning about types and
preconditions with reasoning about other properties. In this way, 
it is possible to treat partial functions that have preconditions
of unlimited complexity.
We show that, in spite of its increased complexity,
the semantics is still a natural generalization of first-order logic
with simple types. If one does not use the increased expressivity,
the type system is not stronger than classical logic with simple types.

I define two sequent calculi for the new semantics, and prove
that they are sound and complete.
The first calculus follows the semantics closely, and hence
its completeness proof is fairly straightforward.
The second calculus is further away from the semantics, but
more suitable for practical use because it has better proof theoretic
properties. Its completeness can be shown by proving that proofs
from the first calculus can be translated.  

[This](pcl_pre_jar2011.pdf) is a preprint of the paper. 
The final version was published in the Journal of Automated
Reasoning, and can be obtained from 
[Springer](http://www.springerlink.com).

## 2010 

### Classical Logic with Partial Functions 

We introduce a semantics for classical logic with partial
functions. We believe that this semantics is natural.
When a formula contains a subterm in which a function is
applied outside of its domain, our semantics ensures
that the formula has no truth-value,
so that it cannot be used for reasoning.
The semantics relies on order of formulas.
In this way, it is able to ensure
that functions and predicates are properly declared before
they are used.
We define a sequent calculus for the semantics, and prove
that this calculus is sound and complete for the semantics.
The paper appeared in the proceedings of IJCAR 2010. 

[This](pcl_pre_ijcar2010.pdf) is a preprint.

## 2008 

### A small Framework for Proof Checking 

We describe a small framework in which first-order theorem provers
can be used for the verification of mathematical theories.
The verification language is designed in such a way that the
use of higher-order constructs is minimized. In this way,
we expect to be able to take advantage of the first order theorem prover
as much as possible. 

[pdf](paar2008.pdf).

## 2006 

### Geometric Resolution: A Proof procedure based on Finite Model Search 

We present a proof procedure that is complete for first-order
logic, but which can also be used when searching for finite
models. The procedure uses a normal form which is based on
geometric formulas. For this reason we call the procedure
geometric resolution.
We expect that the procedure can be used as an efficient
proof search procedure for first-order logic.
In addition, the procedure can be implemented in such a way that it is
complete for finding finite models.

[Download](ijcar2006.pdf).

### Using Resolution as a Decision Procedure (Habilitation Thesis) 

This habilitation thesis is based on five papers 
that deal with resolution decision procedures.
Resolution is a well-known technique for first-order theorem proving.
It is complete, but it does not terminate in general,
when there exists no proof. However, in many cases, 
resolution can be modified in such a way that it becomes a 
decision procedure for certain subclasses of first-order logic.  

We have studied several aspects related to the use
of resolution as decision procedure. 
The first two papers introduce resolution decision procedures for the 
guarded fragment with and without equality. 
The third paper builds on the decision procedure for the guarded 
fragment. Using the decision procedure, modal logics can be decided
by translation into the guarded fragment with the relational
translation. We have extended the standard relational
translation of modal logics, so that more modal logics can be 
translated into the guarded fragment. In particular, modal
logic S4 can now be translated. Before, 
only translations into extensions of the guarded fragment existed.
The fourth paper shows that a standard refinement of resolution, 
which uses a liftable order, can be used to obtain a decison procedure 
for the E-plus class. This was posed as an open problem in 
(Resolution Methods for the Decision Problem,
 C. Fermueller, A. Leitsch, T. Tammet, N. Zamov, Springer Verlag 1993)

The fifth paper introduces a resolution-based decision procedure for the
two-variable fragment with equality. The procedure consists 
of three stages: Saturation under resolution, elimination of equality, 
and one more time saturation under resolution. 

[Download](habilitationschrift.pdf).

### Sonstige Arbeiten (Additional Works) 

In addition to the main habilitation thesis, one has to submit
5 additional publications (sonstige Arbeiten).
They are collected in a supplement, which you may download 
free of charge as 
[pdf](sonstig.pdf).

## 2003 

### Deciding Regular Grammar Logics with Converse through First-Order Logic 

#### (Joint work with Stephane Demri, LSV Paris, France) 

We provide a simple translation of the satisfiability problem
for regular grammar logics with converse into $ \GF^2, $ which is the
intersection of
the guarded fragment and the $ 2 $-variable fragment
of first-order logic.
This translation is theoretically interesting because it translates
modal logics with certain frame conditions into first-order logic,
without explicitly expressing the frame conditions.

A consequence of the translation is that the general satisfiability
problem for regular grammar logics with converse is in EXPTIME.
This extends a previous result of the first author
for grammar logics without converse.
Using the same method, we show how some other modal logics can
be naturally translated into
$ \GF^2, $ including nominal tense logics and intuitionistic
logic.
In our view, the results in this paper show that the natural
first-order fragment corresponding to regular grammar logics is simply
$ \GF^2 $ without extra machinery such as fixed point-operators.
Download as [pdf](newtocl.pdf).


## Implementing the Clausal Normal Form Transformation with Proof Generation


The paper describes how I intend to implement the clausal
normal form transformation with proof generation described 
in the paper below. The paper
introduces a convenient datastructure for sequent proofs, 
which allows easy proof checking and proof normalization.
[Download](wil2003_proofs.pdf).


### Translation of Resolution Proofs into Short First-Order Proofs without Choice Axioms 

We present a way of transforming a resolution proof containing
Skolemization into a natural deduction proof of the same formula
but not using Skolemization. The size of the
proof increases only moderately (polynomially).
This makes it possible to translate the output of a resolution
theorem prover into a purely first-order proof that is moderate
in size.
Download [draft](infcomp2003_nochoice.pdf).

### Subsumption of concepts in FL0 for (cyclic) terminologies with respect to descriptive semantics is PSPACE-complete. 

The paper solves an open problem concerning the complexities of
the simple description logic FL0. FL0 is the description logic
which allows only conjunction and universal value restriction.
We show that subsumption in
this logic is PSPACE-complete under the descriptive semantics. 
The descriptive semantics is the semantics that one obtains if 
one interprets definitions
as simple first-order equivalences. (The other two possibilities
are to interpret definitions as least fixed points, or greatest fixed 
points)
[Download](DL2003_SubDL.pdf).


## Deciding the Guarded Fragments by Resolution 
### (joint work with Maarten de Rijke, University of Amsterdam) 

We give resolution based decision procedures for both
the strictly guarded fragment and the loosely guarded
fragment of first-order logic. We prove that the
decision procedures are in 2EXPTIME, which is theoretically
optimal. 
[Download](rdgf1999_rdgf.pdf).


## 2002 

### Automated Proof Construction in Type Theory using Resolution 
#### (joint work with Marc Bezem, Dimitri Hendriks) 

We provide techniques to integrate resolution logic with equality
in type theory. The results may be rendered as follows:

 
- A clausification procedure in type theory, equipped with
  a correctness proof, all encoded using higher-order primitive recursion.
- A novel representation of clauses in minimal logic
  such that the $ \lambda $-representation of resolution steps
  is linear in the size of the premisses.
- Availability of the power of resolution theorem provers in interactive 
  proof construction systems based on
  type theory

Download [pdf](blinc2002_blinc.pdf).

### Extraction of Proofs from the Clausal Normal Form Transformation 

We give techniques for extracting proofs from the
Clausal Normal Form transformation. We discuss and solve three
technical problems:


- How to handle the introduction of definitions and Skolem functions.
- How to generate short (linear size) proofs.
- How to handle optimized Skolemization. We reduce it
  to standard Skolemization.

[Download](csl2002_paper.pdf).


## 2001 

### Splitting through New Proposition Symbols 

This paper presents ways of simulating splitting through
new propositional symbols. The contribution of the paper
is that the method presented here does not loose backward
redundancy.
We give a general method of obtaining a calculus with splitting
by adjoining splitting symbols to an arbitrary resolution refinement.
We then prove a relative completeness theorem: Every saturated
set of clauses of the resolution calculus with adjoined
proposition symbols contains a saturated set of the original
resolution refinement without adjoined symbols.
[Download](lpar2001_splitting.pdf).


## 2000 

### Datastructures for Resolution 
#### (This is unpublished) 

The paper presents the benchmark tests out of which Bliksem is
grown. The first part compares various ways of implementing terms 
relative to unification and matching. 
The second part compares different ways of implementing substitutions.
The third part compares three ways of implementing discrimination trees.
The paper ends with a description of a subsumption algorithm. 
[Download](2000benchmarks.pdf).


## 1999 

### Translation of S4 and K5 into GF and 2VAR 
#### (This is unpublished) 

This short note gives a method of translating S4 and K5 into the 
intersection
of GF and 2VAR through the introduction of new symbols.
[Download](s4.pdf).

### A Superposition Decision Procedure for the Guarded Fragment with Equality

We give a decision procedure for the
guarded fragment with equality.
The procedure is based on resolution with superposition.
The relevance of the guarded fragment lies in the fact
that many modal logics can be translated into it.
In this way the guarded fragment acts as a framework explaining
some of the nice properties of these modal logics.
By constructing an implementable decision procedure for
the guarded fragments we define an effective procedure
for deciding these modal logics.
It is surprising to see that one does not need any sophisticated
simplification and redundancy elimination method to make superposition
terminate on the class of clauses that is obtained from the clausification
of guarded formulas. Yet the decision procedure obtained
is optimal with regard to time complexity.


## 1997 

### A Classification of Non-Liftable Orders for Resolution 

This paper tries to solve the problem of completeness of resolution
restricted by non-liftable orders that cannot be modelled by the 
resolution game.
Various types of non-liftability are distinguished and combined with
various corresponding types of subsumption. All but one of the 
meaningful combinations are solved.
The remaining case is still open. 

Download [paper](nonlift97.pdf).
The paper was published at CADE 97.  



## 1995 

### Thesis (October 1995, Delft University of Technology, the Netherlands) 

#### The resolution game 

Main contribution of the thesis is the 
__resolution game__ .
The resolution game is a game that can be played between two players,
based on a set of ordered clauses. 
The __opponent__ tries to derive the
empty clause, using ordered resolution and factoring.
The __defender__ tries to disturb
the opponent by changing the order at arbitrary moments. 
The main theorem states that under certain restrictions,
the opponent has a winning strategy (i.e. can always derive
the empty clause) if and only if the clause set is unsatisfiable.


#### Non-liftable Orders 
 
The resolution game can be used for proving completeness
of resolution with non-liftable orders. Non-liftable orders are orders
that are not preserved by substition, i.e. they do not always satisfy
A < B implies Theta(A) < Theta(B).
The standard method of proving completeness (making use of lifting)
does not work for such orders.
With the resolution game, completeness can be proven for some such
orders. 

#### Resolution Based Decision Procedures 

The main application of non-liftable orders is in
*resolution based decision procedures*.
These are resolution restrictions that are guaranteed to terminate
on certain subsets of first-order logic. In my thesis, two 
decision procedures are developed, one for the E+ -class, and one
for the two-variable fragment (without equality).  


#### Maslov's Method 

Another (smaller) contribution of the thesis is that it clarifies
the relation between Maslov's inverse method and resolution. 
Most resolution calculi work top-down. They decompose a formula
into clauses, resolving upon conflicts between clauses.  

Using Maslov's method, it is very easy to obtain a resolution
calculus for every logic that has a cut-free, complete sequent calculus.
However, the resolution calculi that are obtained in this way are
bottom-up, i.e. working from the axioms towards the goal. 

In my thesis, I show that many sequent calculi have a 
__reversal__, which is obtained by 
exchanging axioms and goal, and reversing the direction of the rules.
If one applies Maslov's method on the reversed sequent calculus,
one obtains a top-down resolution calculus. 

You may download [the thesis](proefschrift_proefschrift.pdf) free
of charge if you promise to read it completely.

## 1994 

### Resolution Games and Non-Liftable Resolution Orderings 

This paper introduces the resolution game and proves the completeness
of resolution with orders that are descending. An order < is
descending if always 
A Theta < A, whenever A Theta is a real instance of A.
The completeness proof of the resolution game in this paper is 
very rude. It is based on the analysis of saturated sets. 
The first completeness proof, which is given in my thesis,
is uses intricate combinations of winning strategies, and is much nicer, 
but also more complicated. 

Download [paper](nonlift94.pdf). 
The paper was published at CSL 94. 



