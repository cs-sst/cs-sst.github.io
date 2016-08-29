<div class="container" markdown="1">
<div class="header" markdown="1">Ben Tyler [+]
</div>
<div class="content" markdown="1" style="min-height: 200px;">
{% include image.html url="/images/tyler.jpg" align="right" %}

Associate Professor, Acting Chair

1. Modeling Language Design - My involvement in this area started in 2006, where I was tasked with implementing the Rosetta Systems-Level Design Language (SLDL).  The language itself was proposed in the late 1990s by people who were into hardware design.  Their goal was to create a flexible language that could be used to model different aspects of hardware, but the application areas for this is much wider.  What is technically interesting about Rosetta is its ability to modify its own semantics through special reflective "domain" constructs.<br/>
Due to the heavyweight nature of the language, implementing full Rosetta is not feasible for a senior project.  However, implementing a lightweight version of Rosetta, or preferably a similar type of language that isn't directly tied to Rosetta, would make for an interesting project.  Students would be responsible for aspects of overall language design (what features and syntax?), as well as implementation (parsing, typechecking, executing, etc.)  The tricky part is to find a pragmatic way to approach reflection in the language - it needs to be both easy to use and understand, but not so limited as to be useless for real modeling tasks.

Links to get you thinking:<br/>
Rosetta SLDL:  [http://www.rosetta-lang.org](http://www.rosetta-lang.org) <br/>
Metaobject Protocol (an approach to reflective OO):  http://en.wikipedia.org/wiki/The\_Art\_of\_the\_Metaobject\_Protocol<br/>
Aspect-Oriented Programming (related to the idea of reflection, though used for adding features to Java programs): http://eclipse.org/aspectj/

2. Design Pattern Languages - Part of my Ph.D work was in this area, where we tried to formally specify design patterns, and then use these specifications to generate monitoring code that could be used for detecting specification violations.  The main questions we looked at were:<br/>
a) Can we provide precise specifications about what a particular Design Pattern does?<br/>
b) Can we statically check or dynamically test if a system properly implements a Design Pattern?<br/>
c) How do we tie together a general description of a Design Pattern, and how it is realized in a specific system?<br/>
I haven't looked at this work in a while, but I think it still may bear some fruit (e.g., conference papers.)  Some links for consideration:<br/>

A related approach is to actually build Design Pattern facilities right into your programming language (http://c2.com/cgi/wiki?PatternLanguagesOfProgramDesign)<br/>
Design Patterns could be potentially supported via "add-ons" http://www.cs.ubc.ca/labs/spl/papers/2002/oopsla02-patterns.pdf
Jason O. Hallstrom also worked on this problem (we had the same Ph.D advisor): http://people.cs.clemson.edu/~jasonoh/Jasoni\_O.\_Hallstrom/JOH\_-\_Home.html<br/>

Pattern Language Conference-lots of interesting related (and unrelated) work:  http://www.hillside.net/plop/2014/<br/>

3. Instructional Tech - We have already gone ahead and "flipped" ([https://en.wikipedia.org/wiki/Flipped_classroom](https://en.wikipedia.org/wiki/Flipped_classroom)) the classroom for CSCI 151 and 152.  For this potential project, we want to investigate how we might further improve the classroom experience in our CS courses.  I don't have any particular ideas regarding this right now, but if you have an idea, feel free to try to convince me this would be a worthwhile senior project.  One thing that might be interesting is to create some specialized software to help students learn particular concepts for a course.<br/>

4. Intelligent Agent Framework - Okay, here's the scenario:  we have numerous autonomous agents acting in an uncertain and hostile environment, and they must cooperate in some fashion to meet specified goals.  Fighting wildfires with UAVs, underwater exploration and/or recovery using UUVs, and battlefield combat and recon operations are all examples that fit the scenario.  This project has two components that need to be addressed:<br/>

1)  We need to develop algorithms for intelligent decision-making in non-ideal situations<br/>
2)  We need something to help visualize and evaluate how these algorithms work when deployed<br/>

For this project, we would need to find a 3D visualization framework for showing what is going on in the scenario environment.  We would also need to realistically simulate the entities in the environment, and implement things like physics, dynamics, sensing (observability), constraints on the agents, etc.  On the more technical side of things, we would have to develop the decision-making algorithms, which could be based on Neuro-Dynamic Programming (NDP), NFDP, Rule-based systems, machine learning (?), or something else.<br/>

Helpful links to people I've worked with on this problem:<br/>
Nick Hanlon's M.S. thesis (https://etd.ohiolink.edu/ap/10?0::NO:10:P10\_ACCESSION\_NUM:ucin1321370261)<br/>
Kelly Cohen's work on SIERRA can be found at the following web link (http://phys.org/news/2014-01-dont-dawn-dronessomeday-life-video.html) <br/>

Frameworks listing on Wikipedia:<br/>

https://en.wikipedia.org/wiki/Comparison\_of\_agent-based\_modeling\_software<br/>

5. Other Potential Projects <br/>

Cognitive Architectures (SOAR) (http://sitemaker.umich.edu/soar/home)<br/>
Formal Logics for programming languages<br/>
Model Checking applications<br/>
Testing Object-Oriented Software<br/>

</div>
</div>
