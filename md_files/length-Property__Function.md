## [length Property (Function) (JavaScript)](length-Property__Function.html)

### Introduction 

 Gets the number of arguments defined for a function.

### Syntax 

```
functionName .length
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <i>functionName</i> is the name of the function.
  </p>
  <p xmlns:util="util">
    The <b>length</b> property of a function is initialized by the scripting engine to the number of arguments in the function's definition when an instance of the function is created.
  </p>
  <p xmlns:util="util">
    What happens when a function is called with a number of arguments different from the value of its <b>length</b> property depends on the function.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>length</b> property:
</p>

```
function ArgTest(a, b){ var s = ""; s += "Expected Arguments: " + ArgTest.length; s += "&lt;br /&gt;"; s += "Passed Arguments: " + arguments.length; return s; } document.write(ArgTest(1, 2)); //
Output: // Expected Arguments: 2 // Passed Arguments: 2
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
    <span sdata="link" xmlns:util="util"><a href="efc7a1ee-0880-4f05-b0f2-808f31a4af1d.htm">arguments Property (Function) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e1c6377c-2e84-440a-9660-f1f512e4a938.htm">length Property (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7dbd4a0e-c24e-4561-9b5b-e75e649a10a4.htm">length Property (String) (JavaScript)</a></span>
  </div>
</div>

