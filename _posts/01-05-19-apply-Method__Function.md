---
title: apply Method (Function) (JavaScript)
---

### Introduction 

 Calls the function, substituting the specified object for the this value of the function, and the specified array for the arguments of the function.

### Syntax 

```
apply([thisObj [,argArray ]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">thisObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The object to be used as the <span sdata="langKeyword" value="this"><span class="keyword">this</span></span> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">argArray</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A set of arguments to be passed to the function.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">argArray</span> is not a valid object, then an "Object expected" error occurs.
  </p>
  <p xmlns:util="util">
    If neither <span class="parameter" sdata="paramReference">argArray</span> nor <span class="parameter" sdata="paramReference">thisObj</span> are supplied, the original <span sdata="langKeyword"
    value="this"><span class="keyword">this</span></span> object is used as <span class="parameter" sdata="paramReference">thisObj</span> and no arguments are passed.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use the apply method.
</p>

```
function callMe(arg1, arg2){ var s = ""; s += "this value: " + this; s += "&lt;br /&gt;"; for (i in callMe.arguments) { s += "arguments: " + callMe.arguments[i]; s += "&lt;br /&gt;"; } return s; }
document.write("Original function: &lt;br/&gt;"); document.write(callMe(1, 2)); document.write("&lt;br/&gt;"); document.write("Function called with apply: &lt;br/&gt;");
document.write(callMe.apply(3, [ 4, 5 ])); // Output: // Original function: // this value: [object Window] // arguments: 1 // arguments: 2 // Function called with apply: // this value: 3 //
arguments: 4 // arguments: 5
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
    <span sdata="link" xmlns:util="util"><a href="d3834767-203c-475e-848c-95c423ba15b6.htm">Function Object (JavaScript)</a></span>
  </div>
</div>

