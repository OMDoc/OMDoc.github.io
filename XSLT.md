---
layout: default
title: OMDoc XSLT
---

#XSLT Stylesheets for OMDoc

As OMDoc is an XML application, we can use the [XSL(T)](http://www.w3.org/Style/XSL) style sheet language for transforming OMDoc documents into other formats.

As mathematics heavily relies on notational conventions for symbols and expressions, these
style sheets should be augmented by templates that can be generated specifically for the
source document to get good results. OMDoc provides a common architecture for this, which
we have used in the examples on this page.

 
## Stylesheets for presenting OMDoc Documents to humans

* in HTML, [omdoc2html.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2html.xsl) (uses CSS for styling [omdoc-default.css](https://github.com/OMDoc/OMDoc-1.2/lib/omdoc-default.css)) 
* in LaTeX, [omdoc2tex.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2tex.xsl) (uses LaTeX package [omdoc.sty](https://github.com/OMDoc/OMDoc-1.2/lib/omdoc.sty)).  
 The BibTeX entry for a document can be extracted by [omdoc2bib.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2bib.xsl) (use with care). 
* in presentation [MathML](http://www.w3c.org/MATH), [omdoc2pmml.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2pmml.xsl) (use a MathML-enabled browser like [Mozilla](http://www.mozilla.org/projects/mathml) to view). Note that all of these are based on [omdoc2share.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2share.xsl) 

 
## Stylesheets for transforming them into machine prover input

* for LambdaClam: [omdoc2lclam.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2lclam.xsl) 
* for the [INKA](http://github.com/theoremprover-museum/InKa/) inductive theorem prover [omdoc2dgrl.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2dgrl.xsl) 
* for the [TPS](http://gtps.math.cmu.edu/tps.html)  higher-order theorem prover [omdoc2tps.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2tps.xsl) 
* for the [OMEGA](http://github.com/theoremprover-museum/OMEGA) mathematical assistant: [omdoc2post.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2post.xsl) 
* for interfacing with  OpenMath components: 
  * [cd2omdoc.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/cd2omdoc.xsl) generates OMDoc from  OpenMath Content dictionaries. 
  * [omdoc2cd.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2cd.xsl) generates CDs from OMDocs; use  [omdoc2defmp.xsl](https://github.com/OMDoc/OMDoc-1.2/xsl/omdoc2defmp.xsl), to generate defmp files 
