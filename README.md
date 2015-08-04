# learn-tt

Lot's of people seem curious about type theory but it's not at all
clear how to go from no math background to understanding "Homotopical
Patch Theory" or whatever the latest cool paper is. In this repository
I've gathered links to some of the resources I've personally found
helpful.

Please keep in mind these disclaimers

 - I'm still learning
 - The resources are biased towards what I find interesting: pure type
   theory and proof theory. Lacking is references more focused on
   verification, security, any of the other countless interesting
   facets of programming languages

## Reading Advice

Here's how I read most of the resources listed below

 1. Start with the textbooks, they're mostly self-contained and are
    much clearer about their audience. They'll also give you the
    background you'll need to read other papers.

 2. When reading a paper, if you get stuck see what the paper
    references on the subject. Continue to read references until you
    eventually understand what's going on and then return to the
    paper. You'll learn *something* at least

 3. Implement often. I had a hard time understanding a lot of these
    topics originally until I actually sat down and wrote small
    compilers/type checkers for the languages they describe. Plus it's
    fun.

 4. Skim heavily. If you try to read a paper in depth the first time
    it takes twice as long as skimming it once and reading it more
    thoroughly a second time.

## The Resources

### Text books

 - Practical Foundations of Programming Languages (PFPL)

    I reference this more than any other book. It's a very wide
    ranging survey of programming languages that assumes very little
    background knowledge. A lot people prefer the next book I mention
    but I think PFPL does a better job explaining the foundations it
    works from and then covers more topics I find interesting.

    * Online copy
    * Dead-tree copy

 - Types and Programming Languages (TAPL)

    Another very widely used introductory book (the one I learned
    with). It's good to read in conjunction with PFPL as they
    emphasize things differently. Notably, this includes descriptions
    of type inference which PFPL lacks and TAPL lacks most of PFPL's
    descriptions of concurrency/interesting imperative languages. Like
    PFPL this is very accessible and well written.

   * Online supplements
   * Dead-tree copy

 - Advanced Topics in Types and Programming Languages (ATTAPL)

   Don't feel the urge to read this all at once. It's a bunch of fully
   independent but excellent chapters on a bunch of different
   topics. Read what looks interesting, save what doesn't. It's good
   to have in case you ever need to learn more about one of the
   subjects in a pinch.

   * Dead-tree copy

### Proof Assistants

One of the fun parts of taking in an interest in type theory is that
you get all sorts of fun new programming languages to play with. These
are useful on two fronts

 - You can use them to formalize what you've seen so far
 - Actually working in the type theory gives you a much better
   understanding for it
 - You can tie in your software-engineering experience with all this
   math stuff.

Some major proof assistants are

 - Coq

    Coq is one of the more widely used proof assistants and has the
    best introductory material by far in my opinion.

    * Official site
    * Software Foundations
    * Certified Programming with Dependent Types
    * The paper on the calculus of constructions
    * The paper on the calculus of inductive constructions (What Coq
      is based on)

 - Agda

    Agda is in many respects similar to Coq, but is a smaller language
    overall. It's relatively easy to learn Agda after Coq so I
    recommend doing that. Agda has some really interesting advanced
    constructs like induction-recursion.

    * Official site
    * Tutorial
    * Records tutorial
    * Conor McBride's fun Agda code

 - Idris

    It might not be fair to put Idris in a list of "proof assistants"
    since it really wants to be a proper programming language. It's
    one of the first serious attempts at writing a programming
    language with dependent types *for actual programming* though.

    * Official site
    * Quick tutorial
    * Edwin Brady's fun talks
    * David Christiansen's cool talks

 - Twelf

    Twelf is by far the simplest system in this list, it's the
    absolute minimum a language can have and still be dependently
    typed. All of this makes it easy to pick up, but there are very
    few users and not a lot of introductory material which makes it a
    bit harder to get started with. It does scale up to serious use
    though.

    * Official site
    * Wiki Tutorials
    * My tutorial
    * The paper on LF, the underlying system of Twelf

### Type Theory

 - The Works of Per Martin-Löf

   Per Martin-Löf has contributed a *ton* to the current state of
   dependent type theory. So much so that it's impossible to escape
   his influence. His papers on Martin-Löf Type Theory (he called it
   Intuitionistic Type Theory) are seminal.

   * 1971
   * Girard's proof that 1971's MLTT was inconsistent (This proves
     `Type : Type` is broken)
   * 1972
   * 1979
   * 1984

 - The Works of John Reynold's

   John Reynold's works are similarly impressive and always a pleasure
   to read.

   * Types, Abstraction and Parametric Polymorphism (Parametricity for
     System F)
   * A Logic For Shared Mutable State

 - Computational Type Theory

   While most dependent type theories (like the ones found in Coq,
   Agda, Idris..) are based on Martin-Löf later intensional type
   theories, computational type theory is different. It's a direct
   descendant of his extensional type theory that has been heavily
   developed and forms the basis of NuPRL nowadays. The resources
   below describe the various parts of how CTT works.

   * Type Theory and its Meaning Explanations
   * A Non-Type-Theoretic Definition of Martin-Löf’s Types
   * Constructing a type system over operational semantics (Similar to
     the above, they're helpful to read together)
   * Equality in Lazy Computation System (of general interest)
   * Naive Computational Type Theory
   * Innovations in CTT using NuPRL

### Proof Theory

 - Frank Pfenning's Lecture Notes

    Over the years, Frank Pfenning has accumulated lecture notes that
    are nothing short of heroic. They're not so bad to read and
    almost as good as being in one of his lectures.

    * Introductory Course
    * Linear Logic
    * Modal Logic

### Category Theory

Learning category theory is necessary to understand some parts of type
theory. It's definitely not necessary to understand all of it though!
If you decide to study categorical semantics, realizability, or domain
theory eventually you'll have to buckledown and learn a little at
least. It's actually really cool math so no harm done!

 - Category Theory for Computer Scientists

   This is the absolute smallest introduction to category theory you
   can find that's still useful for a computer scientist. It's very
   light on what it demands for prior knowledge of pure math but
   doesn't go into too much depth.

   * Early version available online
   * Dead-tree version

 - Category Theory

   One of the better introductory books to category theory in my
   opinion. It's notable in assuming relatively little mathematical
   background and for covering quite a lot of ground in a
   readable way.

   * Dead-tree version

 - Ed Morehouse's Category Theory Lecture Notes

   Another valuable piece of reading are these lecture notes. They
   cover a lot of the same areas as "Category Theory" so they can help
   to reinforce what you learned there as well giving you some of
   the author's perspective on how to think about these things.

   * Online copy

### Other Goodness
