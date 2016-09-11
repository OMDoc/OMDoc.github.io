---
layout: default
title: OMDoc1.6
---
# OMDoc 1.6

OMDoc1.6 is the first step towards [OMDoc2.0](../OMDoc2.0), the radically redesigned and
simplified version of the OMDoc format.
 
## Changes to OMDoc1.3
 
In a nutshell, we have the following changes now.

* we have two RelaxNG schemata omdoc-strict.rnc  and omdoc.rnc (for pragmatic OMDoc). 
* I have updated omdoc/examples/omstd/arith1.omdoc to validate in the new schema (but there are still inputs missing at the therory level). 
* Florian's MMT elements are allowed everywhere (but is extended by an informal level and metadata) 
* Most of [OMDoc1.2](OMDoc1.2) is also allowed where it used to be. 
* We are getting rid of the ```<OMOBJ>``` elements, i.e we directly allow the ```OMOBJ``` children there. This makes CMPs much nicer to write. 
* more specical-case attributes like @type are now interpreted as pragmatic versions of RDFa metadata. 
* The OMDoc Spec now comes with a set of format-level CDs (in the source:trunk/doc/spec/cds directory) for metadata ontologies and foundational theories. 

## Ongoing Work
 
The work on OMDoc1.6 is public, the changes are reflected in the
[source:trunk/doc/spec/main.pdf OMDoc1.6 specification]. Upcoming changes are discussed as
TRAC tickets with the [milestone:OMDoc1.6 OMDoc1.6 milestone]; see the
[report:10 development roadmap]. If you are interested in participating in the discussion,
please feel free to add yourselves to the cc fields of the respective issues.
