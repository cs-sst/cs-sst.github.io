---
layout: page
title: Faculty Members
permalink: /faculty/nivelle
---

# Hans de Nivelle, School of Science and Techology 

## Research Interests

My research interests are
*automated theorem proving*, 
*verification*, *proof theory*, 
and *implementation*.


- [Publications](nivelle/publications/index).
- [Talks](nivelle/talks/index). 
- [Implementation](nivelle/implementation/index).

## Committee Memberships

- [IJCAR 2018](http://ijcar2018.org), Oxford, UK, 14-17 July 2018.
- Member of the [TABLEAUX](http://www.tableaux-ar.org) steering committee.
   
## Past Committee Memberhips

- [TABLEAUX 2017](http://tableaux2017.cic.unb.br/),
   Brasilia, 25-29 september 2017.
- [CADE 26](http://www.cse.chalmers.se/~myreen/cade-26/index.html),
   Gothenburg, 6-11 August 2017.
   
## Teaching

For teaching, I refer to [my previous homepage](http://www.ii.uni.wroc.pl/~nivelle/teaching/index.html) in
[Wroclaw](https://en.wikipedia.org/wiki/Wroc%C5%82aw).

## Conferences Organized

I organized <a href = "http://cade23.ii.uni.wroc.pl">CADE 23</a>, 
<a href = "http://tableaux2015.ii.uni.wroc.pl">TABLEAUX 2015</a>, and
<a href = "http://frocos2015.ii.uni.wroc.pl/">FroCoS 2015</a> in
Wroclaw, Poland.


## Quaternion Finder

Build your own [Quaternion Finder](nivelle/quaternion_finder.pdf)! 
Thanks to Tomasz Wierzbicki for the typesetting. 

The cube can also be used for finding (the rotations of)
transformations between different coordinate systems as follows:

1. Align the cube with coordinate system C1.
1. Find the position of (1;0,0,0) on the cube.
1. Align the cube with coordinate system C2.
1. The quaternion can be read off from the place where
   (1;0,0,0) was found in Step 2.

#### Example 

What quaternion represents the eye coordinates
of a pilot, relative to the coordinate system of his plane?

Assume that you are the pilot. Airplane coordinates have
X pointing forward, Y to the right, Z down. In this orientation,
(1;0,0,0) is at the bottom of the cube to the right.

In your eye coordinates, X will be to the right, Y will be upwards,
Z will be pointing behind you.
If you align the cube, bottom right now contains the
quaternion (1;-1,-1,1).

## Grants

- Holder of NCN (Narodowe Centrum Nauki)
   grant 'Decision Procedures for Verification'
   (DEC-2011/03/B/ST6/00346), together
   with [Witold Charatonik](http://www.ii.uni.wroc.pl/~wch).

- Started on 01.03.2016:
   Zastosowania logiki z funcjami częściowymi.
   (Applications of Logic with Partial Functions).
   [In Polish](nivelle/295596-pl.pdf) / [In English](nivelle/295596-en.pdf).


## Picture

{% include image.html url="/images/nivelle.jpg" align="right" %}

