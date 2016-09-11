---
layout: default
title: OMDoc Format
---
# The OMDoc Format

OMDoc is a markup format and data model for Open Mathematical Documents. It serves as semantics-oriented representation format and ontology language for mathematical knowledge.
 
## Multi-level Content Markup
 
OMDoc differs from the presentation-based approaches surveyed in this status report on
[Math on the Web](http://www.dessci.com/en/reference/webmath/) in that it
concentrates on representing the meaning of mathematical formulae instead of their
appearance. OMDoc is an extension of the [OpenMath](http://www.openmath.org) and
[MathML](http://www.w3.org/TR/MathML3/). It extends these formats by markup for the
document, statement and theory level of mathematical documents, so that the document
author can specify them and the consumer (an OMDoc reader or a mathematical software
system) can take advantage of them.

This allows to develop semantics-based added-value services for displaying and manipulating mathematical formulae and structured documents. [more](../toolsprojects)
 
## Design Goals: the OMDoc format aims to

1. be 'ontologically uncommitted' (like the [OpenMath](http://www.openmath.org) format), so that it can serve as an 'integration format' for mathematical software systems. 
2. provide a representation format for 'mathematical documents' that combine 'formal' and 'informal' views of all the 'mathematical knowledge' contained in them. 
3. be based on 'sound logic/representational principles' (as not to embarrass the author in front of his colleagues from automated reasoning) 
4. be based on 'structural/content markup' to guarantee both 1. and 2. To ensure manageability of the format OMDoc is a [modular format](../modules) to allow language subsetting, embedding and [extensions](../extensions). 
 
## Status & History
 
The current stable version of the OMDoc format is [OMDoc1.2](../distribution) which was released in December 2001 and is considered the mature state of OMDoc 1. [History](../history)

Work on OMDoc Version 2 has started. [more](../development)
 
## Resources
 
[Examples](../examples), [tools and systems](../toolsprojects), the [OMDoc distribution](../distribution), ...

