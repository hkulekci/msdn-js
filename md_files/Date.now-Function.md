---
title: Date.now Function (JavaScript)
isChild: false
---

## Date.now Function (JavaScript) {datenow_function_javascript_title}

### Introduction 

 Gets the current date and time.

### Syntax 

```
Date .now()
```

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The number of milliseconds between midnight, January 1, 1970, and the current date and time.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The getTime method returns the number of milliseconds between January 1, 1970, and a specified date.
  </p>
  <p xmlns:util="util">
    For information about how to calculate elapsed time and compare dates, see <span sdata="link">Date and Time Calculations (Windows Scripting - JScript)</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>now</b> method.
</p>

```
var start = Date.now(); var response = prompt("What is your name?", ""); var end = Date.now(); var elapsed = (end - start) / 1000; document.write("You took " + elapsed + " seconds" + " to type: " +
response); // Output: // You took &lt;seconds&gt; seconds to type: &lt;name&gt;
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Not supported in installed versions earlier than Internet Explorer 9. However, it is supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7
    standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10 standards. Also supported in Windows Store apps.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="f0da1d4e-337c-497d-9205-093defbc6d3d.htm">getTime Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ce2202bb-7ec9-4f5a-bf48-3a04feff283e.htm">Date Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Date and Time Calculations (Windows Scripting - JScript)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="003747e2-7860-4c96-b129-5180ae0fe745.htm">JavaScript Methods</a></span>
  </div>
</div>

