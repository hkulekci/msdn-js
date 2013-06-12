---
title: arguments Object (JavaScript)
---

### Introduction 

 An object representing the arguments to the currently executing function, and the functions that called it.

### Syntax 

```
[function .]arguments[n ]
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">function</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The name of the currently executing <span sdata="langKeyword" value="Function"><span class="keyword">Function</span></span> object.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">n</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The zero-based index to argument values passed to the <span sdata="langKeyword" value="Function"><span class="keyword">Function</span></span> object.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You cannot explicitly create an <b>arguments</b> object. The <b>arguments</b> object only becomes available when a function begins execution. The <b>arguments</b> object of the function is not an
    array, but the individual arguments are accessed the same way array elements are accessed. The index <i>n</i> is actually a reference to one of the <b>0</b><b><i>n</i></b> properties of the
    <b>arguments</b> object.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>arguments</b> object.
</p>

```
function ArgTest(a, b) { var s = ""; s += "Expected Arguments: " + ArgTest.length; s += "&lt;br /&gt;"; s += "Passed Arguments: " + arguments.length; s += "&lt;br /&gt;"; s += "The individual
arguments are: " for (n = 0; n &lt; arguments.length; n++) { s += ArgTest.arguments[n]; s += " "; } document.write(s); } ArgTest(1, 2, "hello", new Date()) // Output: // Expected Arguments: 2 //
Passed Arguments: 4 // The individual arguments are: 1 2 hello Tues Jan 8 08:27:09 PST 20xx
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="52857c4b-3d56-4500-93ff-4db4729c2578.htm">0...n Properties (arguments) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ad9d4d21-73f0-44f6-8bec-502f3456cd23.htm">callee Property (arguments) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="3cf36823-15bc-489b-a951-24c4923d9dba.htm">length Property (arguments) (JavaScript)</a></span>
  </div>
</div>

