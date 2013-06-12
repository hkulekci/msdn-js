---
title: 0...n Properties (arguments) (JavaScript)
---

### Introduction 

 Returns the actual value of individual arguments from an arguments object returned by the arguments property of an executing function.

### Syntax 

```
[function .]arguments[[0|1|2|...|n ]]
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
      0, 1, 2, <i xmlns:util="util">, n</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Non-negative integer in the range of 0 to <i>n</i> where 0 represents the first argument and <i>n</i> represents the final argument. The value of the final argument <i>n</i> is
        <b>arguments.length-1</b>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The values returned by the 0 . . . n properties are the actual values passed to the executing function. While not actually an array of arguments, the individual arguments that comprise the
    <b>arguments</b> object are accessed the same way that array elements are accessed.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>0 . . .</b> <b><i>n</i></b> properties of the <b>arguments</b> object. To fully understand the example, pass one or more arguments to the
  function:
</p>

```
function ArgTest(){ var s = ""; s += "The individual arguments are: " for (n = 0; n &lt; arguments.length; n++){ s += ArgTest.arguments[n] ; s += " "; } return(s); } document.write(ArgTest(1, 2,
"hello", new Date()));
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="5eb79ca9-bbb8-4a42-aaf5-16a93ecb425f.htm">arguments Object (JavaScript)</a></span>| <span sdata="link"><a href=
    "d3834767-203c-475e-848c-95c423ba15b6.htm">Function Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="3cf36823-15bc-489b-a951-24c4923d9dba.htm">length Property (arguments) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="fdc8e1c9-0dac-4e1b-ba3a-11073c37ef63.htm">length Property (Function) (JavaScript)</a></span>
  </div>
</div>

