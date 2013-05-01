## [length Property (arguments) (JavaScript)](length-Property__arguments.html)

### Introduction 

 Returns the actual number of arguments passed to a function by the caller.

### Syntax 

```
[function .]arguments.length
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The optional <i>function</i> argument is the name of the currently executing <span sdata="langKeyword" value="Function"><span class="keyword">Function</span></span> object.
  </p>
  <p xmlns:util="util">
    The <b>length</b> property of the <b>arguments</b> object is initialized by the scripting engine to the actual number of arguments passed to a <span sdata="langKeyword" value=
    "Function"><span class="keyword">Function</span></span> object when execution begins in that function.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>length</b> property of the <b>arguments</b> object. To fully understand the example, pass more arguments to the function than the 2 arguments
  expected:
</p>

```
function ArgTest(a, b){ var s = ""; s += "Expected Arguments: " + ArgTest.length; s += "&lt;br /&gt;"; s += "Passed Arguments: " + arguments.length; document.write (s); }
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
    <span sdata="link" xmlns:util="util"><a href="efc7a1ee-0880-4f05-b0f2-808f31a4af1d.htm">arguments Property (Function) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e1c6377c-2e84-440a-9660-f1f512e4a938.htm">length Property (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7dbd4a0e-c24e-4561-9b5b-e75e649a10a4.htm">length Property (String) (JavaScript)</a></span>
  </div>
</div>

