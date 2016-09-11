---
layout: default
title: OMDoc FAQ
---
# The OMDoc FAQ (Frequently Asked Questions)

## What is the current stable version of OMDoc

It is version 1.2, it is described on these web pages and in the [OMDoc specification]("http://omdoc.org/pubs/omdoc1.2.pdf").
 
## What is the road-map for further development in OMDoc?
 
The development of OMDoc 2.0 has already begun, this will be a general (backwards-incompatible) overhaul of the document format, that will take all the experiences with OMDoc 1 into account and track all the developments of web standards since OMDoc 1.2. The development proceeds in steps; see the [wiki:DevelopmentPlan Development Plan] for an overview and [roadmap]("https://trac.omdoc.org/OMDoc/roadmap") for a progress report in terms of TRAC tickets. 
 
## Is'nt OMDoc much too verbose?
 
the OMDoc format is mainly intended for machine consumption. You do not want to look/edit it in this form. For viewing, transform it into html or LaTeX (see the [ToolsSystems tools] section, for editing use an OMDoc or xml editor.
 
## Does'nt communication between mathematical services in OMDoc waste bandwidth?
 
If you are concerned about disk space and bandwidth, consider using xml-specific compression tools like [xmill]("http://sf.net/projects/xmill") or [xmlppm]("http://sourceforge.net/projects/xmlppm"). They take document structure into account during compression and very often realize compressed files that are **smaller** than the non-xml/OMDoc format of the data.
 
##How do I edit an OMDoc document?
You have the choice of either

* use the semantic wiki [SWiM]("http://kwarc.info/project/swim/"), which can import and export OMDoc files, and access files in Subversion repositories 
- using a general-purpose editor to edit the straight OMDoc representation in ASCII. Emacs
  supports this with ```nxml-mode``` is a general XML mode that supports RelaxNG
  schemata. There is also a dedicated OMDoc mode that needs some love and affection.
* a specialized XML development environment like  [XML Spy]("http://www.xmlspy.com") 
* One of the main problems while editing OMDoc is to edit the OpenMath Formulae, there are a couple of solutions for this from the [OpenMath home page]("http://www.openmath.org"). 
 
## How can I transform legacy documents into OMDoc?
 
There are some rudimentary [wiki:ToolsSystems tools]. For help on this matter contact the [wiki:MailingLists OMDoc mailing lists]

 
## Is there a mailing list for OMDoc?
 
Yes, we do; see details [wiki:MailingLists here]    

## How can I become involved in OMDoc development?
 
There are multiple possibilities, you can

* extend the set of [OMDoc tools]("tools.html"), or 
* join one of the [wiki:MailingLists Mailing lists], or 
* [file issues]("https://trac.omdoc.org/OMDoc/newticket") in TRAC and join the discussions there, o 
* adopt one of the [wiki:Modules OMDoc Modules] For anything else, just contact the [wiki:MailingLists developer's mailing list] 
