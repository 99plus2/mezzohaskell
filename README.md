There is a fairly large amount of beginner material available for Haskell. Real
World Haskell and Learn You a Haskell each provide a great foundation in the
language, and by now the plethora of monad tutorials has become infamous. There
are also a great quantity of research papers and blog posts focusing on
advanced features of the language.

What's missing is that intermediate stepping stone. Many of the newer language
extensions provided by GHC are of practical use on many projects, but knowledge
of them is not immediately available. While we have many high performance
libraries, it is not always apparent which is the right choice for a specific
task.

The goal of this book is to provide that stepping stone. It is intended to be a
community-driven effort, consisting of writings by many members of the
community. Writing this book is a project which will consist of a few steps:

1. Brainstorming on what should be covered.

2. Organizing the content into a consistent outline.

3. Gathering content from various members of the community.

4. Reviewing and improving the content: both to improve its technical accuracy,
   and to make it more accessible to newcomers.

As it stands now, there are no plans to publish this book, though that may
become relevant. I suppose one issue we should address is how licensing and
book royalties would be worked out. I would recommend that all content have
copyright assigned to a central organization (haskell.org), that it be licensed
under a Creative Commons license, and any profit made from it be donated back
to haskell.org.

# Topics

We still need to determine how the book will flow. The breakdown given below is
not intended to provide an actual outline of the book, but merely to organize
the concepts. It is very likely that we will be introducing language features
(e.g., OverloadedStrings) at the same time as we introduce libraries (e.g.,
text).

## "Core"

* Exception handling
* Asynchronous exceptions
* Basic typeclasses (Monoid, Applicative, Alternative)

## Common techniques

* Monad transformers
    * monad-control
* CPS

## Language extensions

* OverloadedStrings
* ViewPatterns
* PatternGuards
* TypeFamilies
* FunDeps
* MPTC
* GADT
* TemplateHaskell
* QuasiQuotes

## Data structures

* vector
* containers
* unordered-containers
* text
* bytestring

## Serialization

* binary/cereal
* blaze-builder
* blaze-html
* attoparsec
* aeson
* yaml
* xml-conduit

## Other libraries

* system-filepath

## Open debates

* Streaming data
    * conduit
    * iteratee/enumerator
    * pipes
* Typeclasses versus records
* "Good" use of typeclass extensions
* Proper error reporting (Either, Maybe, ErrorT)

## Tools

* cabal
* cabal-dev/virthualenv
* Test framework

## Debugging/optimizing

* hlint
* Debugging
* Profiling
* Finding space leaks
* Strictness annotations
* Pragmas (UNPACK, INLINE, ...)
* Heap profiling

# Organizational questions

* Should the book be kept on Github?

* What format should we use for the content? Markdown, Literate Haskell, LaTeX?

* Should the book have its own Github organization with lots of committers, or
  should everyone create their own fork?
