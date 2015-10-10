# learn-tt

Lots of people seem curious about type theory but it's not at all
clear how to go from no math background to understanding "Homotopical
Patch Theory" or whatever the latest cool paper is. In this repository
I've gathered links to some of the resources I've personally found
helpful.

## Reading Advice

I strongly urge you to start by reading one or more of the textbooks
immediately below. They give a nice self-contained introduction and a
foundation for understanding the papers that follow. Don't get hung up
on any particular thing, it's always easier to skim the first time and
read closely on a second pass.

## The Resources

### Textbooks

 - Practical Foundations of Programming Languages (PFPL)

    I reference this more than any other book. It's a very wide
    ranging survey of programming languages that assumes very little
    background knowledge. A lot people prefer the next book I mention
    but I think PFPL does a better job explaining the foundations it
    works from and then covers more topics I find interesting.

    * [Online copy](http://www.cs.cmu.edu/~rwh/plbook/1sted-revised.pdf)
    * [Dead-tree copy](http://www.amazon.com/Practical-Foundations-Programming-Languages-Professor/dp/1107029570/ref=sr_1_1?ie=UTF8&qid=1439346858&sr=8-1&keywords=practical+foundations+for+programming+languages)

 - Types and Programming Languages (TAPL)

    Another very widely used introductory book (the one I learned
    with). It's good to read in conjunction with PFPL as they
    emphasize things differently. Notably, this includes descriptions
    of type inference which PFPL lacks and TAPL lacks most of PFPL's
    descriptions of concurrency/interesting imperative languages. Like
    PFPL this is very accessible and well written.

   * [Online supplements](http://www.cis.upenn.edu/~bcpierce/tapl/)
   * [Dead-tree copy](https://mitpress.mit.edu/books/types-and-programming-languages)

 - Advanced Topics in Types and Programming Languages (ATTAPL)

   Don't feel the urge to read this all at once. It's a bunch of fully
   independent but excellent chapters on a bunch of different
   topics. Read what looks interesting, save what doesn't. It's good
   to have in case you ever need to learn more about one of the
   subjects in a pinch.

   * [Online supplements](http://www.cis.upenn.edu/~bcpierce/attapl/)
   * [Dead-tree copy](http://www.amazon.com/exec/obidos/ASIN/0262162288/benjamcpierce)

### Proof Assistants

One of the fun parts of taking in an interest in type theory is that
you get all sorts of fun new programming languages to play with. Some
major proof assistants are

 - Coq

    Coq is one of the more widely used proof assistants and has the
    best introductory material by far in my opinion.

    * [Official site](https://coq.inria.fr/)
    * [Software Foundations](http://www.cis.upenn.edu/~bcpierce/sf/current/index.html)
    * [Certified Programming with Dependent Types](http://adam.chlipala.net/cpdt/)
    * [The paper on the calculus of constructions](https://hal.inria.fr/inria-00076024/document)
    * [The paper on the calculus of inductive constructions](http://www.cs.cmu.edu/~fp/papers/mfps89.pdf) (What Coq
      is based on)

 - Agda

    Agda is in many respects similar to Coq, but is a smaller language
    overall. It's relatively easy to learn Agda after Coq so I
    recommend doing that. Agda has some really interesting advanced
    constructs like induction-recursion.

    * [Official site](http://wiki.portal.chalmers.se/agda/pmwiki.php)
    * [Tutorial](http://www.cse.chalmers.se/~ulfn/papers/afp08/tutorial.pdf)
    * [Records tutorial](http://wiki.portal.chalmers.se/agda/pmwiki.php?n=ReferenceManual.RecordsTutorial)
    * [Conor McBride's](https://github.com/pigworker/MetaprogAgda) [fun Agda code](https://github.com/pigworker/CS410-14)

 - Idris

    It might not be fair to put Idris in a list of "proof assistants"
    since it really wants to be a proper programming language. It's
    one of the first serious attempts at writing a programming
    language with dependent types *for actual programming* though.

    * [Official site](http://idris-lang.org/)
    * [Quick tutorial](http://docs.idris-lang.org/en/latest/tutorial/index.html#tutorial-index)
    * [A list of talks on Idris](https://www.youtube.com/watch?v=O1t4xJzrOng)
    * [David Christiansen's cool talk](https://www.youtube.com/watch?v=dP2imvL92sY)

 - Twelf

    Twelf is by far the simplest system in this list, it's the
    absolute minimum a language can have and still be dependently
    typed. All of this makes it easy to pick up, but there are very
    few users and not a lot of introductory material which makes it a
    bit harder to get started with. It does scale up to serious use
    though.

    * [Official site](http://twelf.org/)
    * [Wiki Tutorials](http://twelf.org/wiki/Tutorials)
    * [My tutorial](http://jozefg.bitbucket.org/posts/2015-02-28-twelf.html)
    * [The paper on LF, the underlying system of Twelf](http://citeseer.ist.psu.edu/viewdoc/summary?doi=10.1.1.21.5854)

### Type Theory

 - The Works of Per Martin-Löf

   Per Martin-Löf has contributed a *ton* to the current state of
   dependent type theory. So much so that it's impossible to escape
   his influence. His papers on Martin-Löf Type Theory (he called it
   Intuitionistic Type Theory) are seminal.

    If you're confused by the papers above read the book in the next
    entry and try again. The book doesn't give you as good a feel for
    the various flavors of MLTT (which spun off into different areas
    of research) but is easier to follow.

   * [1972](https://github.com/michaelt/martin-lof/blob/master/pdfs/An-Intuitionistic-Theory-of-Types-1972.pdf?raw=true)
   * [1979](https://github.com/michaelt/martin-lof/blob/master/pdfs/Constructive-mathematics-and-computer-programming-1982.pdf?raw=true)
   * [1984](https://github.com/michaelt/martin-lof/blob/master/pdfs/Bibliopolis-Book-retypeset-1984.pdf?raw=true)

 - Programming In Martin-Löf's Type Theory

   It's good to read the original papers and here things from the
   horses mouth, but Martin-Löf is much smarter than us and it's nice
   to read other people explanations of his material. A group of
   people at Chalmer's have elaborated it into a book.

   * [Online link](http://www.cse.chalmers.se/research/group/logic/book/book.pdf)

 - The Works of John Reynolds

   John Reynolds' works are similarly impressive and always a pleasure
   to read.

   * [Types, Abstraction and Parametric Polymorphism](http://www.cse.chalmers.se/edu/year/2010/course/DAT140_Types/Reynolds_typesabpara.pdf) (Parametricity for
     System F)
   * [A Logic For Shared Mutable State](http://www.cs.cmu.edu/~jcr/seplogic.pdf)
   * [Course notes on separation logic](http://www.cs.cmu.edu/afs/cs.cmu.edu/project/fox-19/member/jcr/www15818As2011/cs818A3-11.html)
   * [Course notes on denotational semantics](http://www.cs.cmu.edu/~jcr/cs819-00.html)

 - Computational Type Theory

   While most dependent type theories (like the ones found in Coq,
   Agda, Idris..) are based on Martin-Löf later intensional type
   theories, computational type theory is different. It's a direct
   descendant of his extensional type theory that has been heavily
   developed and forms the basis of NuPRL nowadays. The resources
   below describe the various parts of how CTT works.

   * [Type Theory and its Meaning Explanations](https://github.com/jonsterling/type-theory-and-its-meaning-explanations)
   * [A Non-Type-Theoretic Definition of Martin-Löf’s Types](http://www.cs.cornell.edu/Info/Projects/NuPrl/documents/Allen/lics87.html)
   * [Constructing a type system over operational semantics](https://www.cs.uoregon.edu/research/summerschool/summer10/lectures/Harper-JSC92.pdf)
     (Similar to the above, they're helpful to read together)
   * [Equality in Lazy Computation System](http://www.nuprl.org/documents/Howe/EqualityinLazy.html) (of general interest)
   * [Naive Computational Type Theory](http://www.nuprl.org/documents/Constable/naive.pdf)
   * [Innovations in CTT using NuPRL](http://www.nuprl.org/documents/Allen/05-jal-final.pdf)

 - Homotopy Type Theory

   A new exciting branch of type theory. This exploits the connection
   between homotopy theory and type theory by treating types as
   spaces. It's the subject of a lot of active research but has some
   really nice introductory resources even now.

   * [The HoTT book](http://homotopytypetheory.org/book/)
   * [Student's Notes on HoTT](https://github.com/RobertHarper/hott-notes)


### Proof Theory

 - Frank Pfenning's Lecture Notes

    Over the years, Frank Pfenning has accumulated lecture notes that
    are nothing short of heroic. They're wonderful to read and almost
    as good as being in one of his lectures.

    * [Introductory Course](http://www.cs.cmu.edu/~fp/courses/15317-f09/)
    * [Linear Logic](http://www.cs.cmu.edu/~fp/courses/15816-s12/)
    * [Modal Logic](http://www.cs.cmu.edu/~fp/courses/15816-s10/)

### Category Theory

Learning category theory is necessary to understand some parts of type
theory. If you decide to study categorical semantics, realizability,
or domain theory eventually you'll have to buckledown and learn a
little at least. It's actually really cool math so no harm done!

 - Category Theory for Computer Scientists

   This is the absolute smallest introduction to category theory you
   can find that's still useful for a computer scientist. It's very
   light on what it demands for prior knowledge of pure math but
   doesn't go into too much depth.

   * [Early version available online](http://repository.cmu.edu/cgi/viewcontent.cgi?article=2846&context=compsci)
   * [Dead-tree version](https://mitpress.mit.edu/index.php?q=books/basic-category-theory-computer-scientists)

 - Category Theory

   One of the better introductory books to category theory in my
   opinion. It's notable in assuming relatively little mathematical
   background and for covering quite a lot of ground in a
   readable way.

   * [Dead-tree version](http://www.amazon.com/Category-Theory-Oxford-Logic-Guides/dp/0199237182/ref=sr_1_1?ie=UTF8&qid=1439348930&sr=8-1&keywords=awodey+category+theory)

 - Ed Morehouse's Category Theory Lecture Notes

   Another valuable piece of reading are these lecture notes. They
   cover a lot of the same areas as "Category Theory" so they can help
   to reinforce what you learned there as well giving you some of
   the author's perspective on how to think about these things.

   * [Online copy](http://www.cs.cmu.edu/~edmo/research/notes/intro_categorical_semantics.pdf)

### Other Goodness

 - Gunter's "Semantics of Programming Language"

   While I'm not as big a fan of some of the earlier chapters, the
   math presented in this book is absolutely top-notch and gives a
   good understanding of how some cool fields (like domain theory)
   work.

   * [Dead-tree version](http://www.amazon.com/Semantics-Programming-Languages-Structures-Foundations/dp/0262071436/ref=sr_1_1?ie=UTF8&qid=1439349219&sr=8-1&keywords=gunter+semantics+of+programming+languages)

 - Abramsky and Jung's "Domain Theory"

   This what I reference nowadays for domain theory. It's a very good
   (if a little dense) introduction covering all the basic mathematics
   necessary to work with domains productively.  It should definitely
   be possible to follow if you've read some of Gunter's book.

   - [CiteSeerX link](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.50.8851)

 - OPLSS

   The Oregon Programming Languages Summer School is a 2 week long
   bootcamp on PLs held annually at the university of Oregon. It's a
   wonderful event to attend but if you can't make it they record all
   their lectures anyways! They're taught be a variety of lecturers
   but they're all world class researchers.

   * [2012](https://www.cs.uoregon.edu/research/summerschool/summer12/curriculum.html)
   * [2013](https://www.cs.uoregon.edu/research/summerschool/summer13/curriculum.html)
   * [2014](https://www.cs.uoregon.edu/research/summerschool/summer14/curriculum.html)
   * [2015](https://www.cs.uoregon.edu/research/summerschool/summer15/curriculum.html)
