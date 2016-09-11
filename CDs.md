---
layout: default
title: OMDoc and OpenMath CDs
---
Content Dictionaries are special documents that define the semantics of symbols. They contain descriptions, mathematical properties, and examples of the concepts represented by these symbols to make their meaning unambiguous. The concept has first been introduced for the [OpenMath](http://www.openmath.org) format, but will also be the basis for the upcoming MathML3 recommendation.

OMDoc is uses content dictionaries in two ways

1. OMDoc uses OpenMath Objects, and in particular OpenMath symbols (```OMS```) to represent objects, these are of the form ```<OMS cd="theo" name="nam">```. The ```cd``` attribute points to a CD ```theo.ocd```, where the symbol with the name ```nam``` is defined. 
2. OMDoc is a a drop-in replacement for CDs, since OMDoc theories specify a superset of the information in a CD. In particular, ```theo.omdoc``` can contain an element ```<symbol name="nam">``` element inside a ```<theory xml:id="nam">``` that specifies the same information. Moreover, OMDoc theories provide powerful primitives for structured theory specification and presentation, so authors may only want to specify OMDocs. 

As a consequence OMDocs may contain definitions of mathematical concepts, which need to be referred to using OpenMath symbols. In particular, documents describing theories even reference symbols they define themselves.

The [OpenMath Society](http://www.openmath.org) has developed a [set of official CDs](http://www.openmath.org/cd/) for central mathematical concepts. They contain a subset, that is isomorphic to the [MathML](http://www.w3.org/Math/) concepts, so that rendering is well-understood. For your convenience, we have converted them [to OMDoc](https://github.com/OMDoc/OMDoc1.2/examples/omstd). This repository contains the omdoc files themselves (they have been slightly edited to iron out some referencing errors in the CDs, and some of them have been augmented by ```<presentation>``` elements).
