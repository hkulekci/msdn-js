---
title: call Method (Function) (JavaScript)
isChild: false
---

## call Method (Function) (JavaScript) {call_method_function_javascript_title}

### Introduction 

 Calls a method of an object, substituting another object for the current object.

### Syntax 

```
call([thisObj [, arg1 [, arg2 [, [, argN ]]]]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">thisObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The object to be used as the current object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arg1, arg2, , argN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A list of arguments to be passed to the method.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>call</b> method is used to call a method on behalf of another object. It allows you to change the <span sdata="langKeyword" value="this"><span class="keyword">this</span></span> object of
    a function from the original context to the new object specified by <span class="parameter" sdata="paramReference">thisObj</span>.
  </p>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">thisObj</span> is not supplied, the <span sdata="langKeyword" value="global"><span class="keyword">global</span></span> object is used as
    <span class="parameter" sdata="paramReference">thisObj</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use the <b>call</b> method.
</p>

```
function callMe(arg1, arg2){ var s = ""; s += "this value: " + this; s += "&lt;br /&gt;"; for (i in callMe.arguments) { s += "arguments: " + callMe.arguments[i]; s += "&lt;br /&gt;"; } return s; }
document.write("Original function: &lt;br/&gt;"); document.write(callMe(1, 2)); document.write("&lt;br/&gt;"); document.write("Function called with call: &lt;br/&gt;"); document.write(callMe.call(3,
4, 5)); // Output: // Original function: // this value: [object Window] // arguments: 1 // arguments: 2 // Function called with call: // this value: 3 // arguments: 4 // arguments: 5
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
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="b36df78e-b14b-46ca-b5cb-de752d80f40a.htm">apply Method (Function) (JavaScript)</a></span>
  </div>
</div>

