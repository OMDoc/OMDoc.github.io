<!doctype html>
<!--[if lt IE 7 ]> <html lang="en-us" dir="ltr" class="no-js ie6"> <![endif]-->
<!--[if IE 7 ]>    <html lang="en-us" dir="ltr" class="no-js ie7"> <![endif]-->
<!--[if IE 8 ]>    <html lang="en-us" dir="ltr" class="no-js ie8"> <![endif]-->
<!--[if IE 9 ]>    <html lang="en-us" dir="ltr" class="no-js ie9"> <![endif]-->
<!--[if (gt IE 9)|!(IE)]><!--> <html lang="en-us" dir="ltr" class="no-js"> <!--<![endif]-->
<head>
  <meta http-equiv="X-UA-Compatible" content="IE=Edge;chrome=1" >
  <meta charset="utf-8">

  <title>CDs || OMDoc Wiki</title>

  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <link rel="stylesheet" href="/public/css/style.css" >
  <link rel="stylesheet" href="/public/css/docs.css" >

</head>
<body>
  <div id="container" class="wikiconvertor"> 
    <b class="border-a"></b>
    <b class="border-b"></b>
    <b class="border-c"></b>
    <b class="border-d"></b>

    <div id="header">
         <h1>OMDoc wiki</h1> 
    </div>

    <div id="body">
      <div class="wikiconvertor-pages">
        <ul>
            <li><a href="abstractDoc_module&#x2F;">abstractDoc_module</a></li>
            <li><a href="CDs&#x2F;">CDs</a></li>
            <li><a href="CodeML&#x2F;">CodeML</a></li>
            <li><a href="Community&#x2F;">Community</a></li>
            <li><a href="cross-ref_revisited&#x2F;">cross ref_revisited</a></li>
            <li><a href="Distribution&#x2F;">Distribution</a></li>
            <li><a href="DocumentOntology&#x2F;">DocumentOntology</a></li>
            <li><a href="examples&#x2F;">examples</a></li>
            <li><a href="extensions&#x2F;">extensions</a></li>
            <li><a href="FAQ&#x2F;">FAQ</a></li>
            <li><a href="history&#x2F;">history</a></li>
            <li><a href="&#x2F;">Home</a></li>
            <li><a href="MailingLists&#x2F;">MailingLists</a></li>
            <li><a href="Modules&#x2F;">Modules</a></li>
            <li><a href="OMDoc1.3&#x2F;">OMDoc1.3</a></li>
            <li><a href="OMDoc1.6&#x2F;">OMDoc1.6</a></li>
            <li><a href="OMDoc2.0&#x2F;">OMDoc2.0</a></li>
            <li><a href="OMDocFormat&#x2F;">OMDocFormat</a></li>
            <li><a href="omdocPortal&#x2F;">omdocPortal</a></li>
            <li><a href="OMDocToolsProjects&#x2F;">OMDocToolsProjects</a></li>
            <li><a href="OpenMath&#x2F;">OpenMath</a></li>
            <li><a href="PageTemplates&#x2F;">PageTemplates</a></li>
            <li><a href="PhysML&#x2F;">PhysML</a></li>
            <li><a href="PresArchitecture&#x2F;">PresArchitecture</a></li>
            <li><a href="RecentChanges&#x2F;">RecentChanges</a></li>
            <li><a href="Repository&#x2F;">Repository</a></li>
            <li><a href="specifications&#x2F;">specifications</a></li>
            <li><a href="Validation&#x2F;">Validation</a></li>
            <li><a href="XSLT&#x2F;">XSLT</a></li>
        </ul>
      </div>

      <div class="wikiconvertor-content wikistyle relative">
        <p>Content Dictionaries are special documents that define the semantics of symbols. They
contain descriptions, mathematical properties, and examples of the concepts represented by
these symbols to make their meaning unambiguous. The concept has first been introduced for
the <a href="http://www.openmath.org">OpenMath</a> format, but will also be the basis for the upcoming
MathML3 recommendation.</p>
<p>OMDoc is uses content dictionaries in two ways</p>
<ol>
<li>OMDoc uses OpenMath Objects, and in
 particular OpenMath symbols (<code><span class="pln">OMS</span></code>) to represent objects, these are of the form
 <code><span class="tag">&lt;OMS</span><span class="pln"> </span><span class="atn">cd</span><span class="pun">=</span><span class="atv">"theo"</span><span class="pln"> </span><span class="atn">name</span><span class="pun">=</span><span class="atv">"nam"</span><span class="tag">&gt;</span></code>. The cd attribute points to a CD <code><span class="pln">theo</span><span class="pun">.</span><span class="pln">ocd</span></code>, where the
 symbol with the name <code><span class="pln">nam</span></code> is defined.</li>
<li>OMDoc is a a drop-in replacement for CDs, since OMDoc theories specify a superset of
 the information in a CD. In particular, <code><span class="pln">theo</span><span class="pun">.</span><span class="pln">omdoc</span></code> can contain an element
 <code><span class="tag">&lt;symbol</span><span class="pln"> </span><span class="atn">name</span><span class="pun">=</span><span class="atv">"nam"</span><span class="tag">&gt;</span></code> element inside a <code><span class="tag">&lt;theory</span><span class="pln"> </span><span class="atn">xml:id</span><span class="pun">=</span><span class="atv">"theo"</span><span class="tag">&gt;</span></code> that specifies
 the same information. Moreover, OMDoc theories provide powerful primitives for structured
 theory specification and presentation, so authors may only want to specify OMDocs.</li>
</ol>
<p>As a consequence OMDocs may contain definitions of mathematical concepts, which need to be
referred to using OpenMath symbols. In particular, documents describing theories even
reference symbols they define themselves.</p>
<p>The <a href="http://www.openmath.org">OpenMath Society</a> has developed a
<a href="http://www.openmath.org/cd/">set of official CDs</a> for central mathematical concepts. They
contain a subset, that is isomorphic to the <a href="http://www.w3.org/Math/">MathML</a>
concepts, so that rendering is well-understood. For your convenience, we have converted
them <a href="https://trac.omdoc.org/browser/branches/omdoc-1.2/examples/omstd">to OMDoc</a>. This
repository contains the omdoc files themselves (they have been slightly edited to iron out
some referencing errors in the CDs, and some of them have been augmented by
<code><span class="tag">&lt;presentation&gt;</span></code> elements).</p>

      </div>

    </div>
  </div>

  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.6.1/jquery.js"></script>
  <script>window.jQuery || document.write('<script src="/public/js/jquery.min.js"><\/script>')</script>

  <script src="//cdnjs.cloudflare.com/ajax/libs/json2/20110223/json2.js"></script>
  <script>window.JSON || document.write("<script src='/public/js/json2.js'>\x3C/script>")</script>

  <script src="//cdnjs.cloudflare.com/ajax/libs/underscore.js/1.1.6/underscore-min.js"></script>
  <script>window._ || document.write("<script src='/public/js/underscore.min.js'>\x3C/script>")</script>

  <script src="//cdnjs.cloudflare.com/ajax/libs/backbone.js/0.5.0/backbone-min.js"></script>
  <script>window.Backbone || document.write("<script src='/public/js/backbone.min.js'>\x3C/script>")</script>

  <script src="/public/js/script.js"></script>

</body>
</html>
