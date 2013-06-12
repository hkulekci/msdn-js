---
title: lastParen Property ($+) (RegExp) (JavaScript)
---

### Introduction 

 Returns the last parenthesized submatch from any regular expression search, if any. Read-only.

### Syntax 

```
RegExp.lastParen
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The object associated with this property is always the global <b>RegExp</b> object.
  </p>
  <p xmlns:util="util">
    The initial value of the <b>lastParen</b> property is an empty string. The value of the <b>lastParen</b> property changes whenever a successful match is made.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>lastParen</b> property:
</p>

```
// Create the regular expression pattern. var re = new RegExp("d(b+)(d)","ig"); var str = "cdbBdbsbdbdz"; // Perform the search. var arr = re.exec(str); // Print the output. var s = "" s += "$1: " +
RegExp.$1 + "&lt;br /&gt;"; s += "$2: " + RegExp.$2 + "&lt;br /&gt;"; s += "$3: " + RegExp.$3 + "&lt;br /&gt;"; s += "input: " + RegExp.input + "&lt;br /&gt;"; s += "lastMatch: " + RegExp.lastMatch +
"&lt;br /&gt;"; s += "leftContext: " + RegExp.leftContext + "&lt;br /&gt;"; s += "rightContext: " + RegExp.rightContext + "&lt;br /&gt;"; s += "lastParen: " + RegExp.lastParen + "&lt;br /&gt;";
document.write(s);
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="7f6b1073-8cbb-49ed-94b6-56833ba663c5.htm">RegExp Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8bd84851-f62f-4eb1-a93d-b67135ea091a.htm">$1...$9 Properties (RegExp) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d8be1ef6-1bf2-43cd-b0b5-567a61eabaad.htm">index Property (RegExp) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="88c6d1d8-56f7-4334-a7eb-e899aec9cda4.htm">input Property ($_) (RegExp) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="c8ae2a13-6dff-4cbe-b662-aca3d66c2a7f.htm">lastIndex Property (RegExp) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d223836d-5235-48a5-a926-d20764ad3f14.htm">lastMatch Property ($&amp;) (RegExp) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="840e56c0-eb7c-461f-bb56-91acff9b5bcf.htm">leftContext Property ($`) (RegExp) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="6999c056-d18c-4583-9dd9-8fbb6d3d0ee7.htm">rightContext Property ($') (RegExp) (JavaScript)</a></span>
  </div>
</div>

