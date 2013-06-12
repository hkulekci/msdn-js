---
title: arguments Property (Function) (JavaScript)
---

### Introduction 

 Gets the arguments for the currently executing Function object.

### Syntax 

```
function .arguments
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">function</span> argument is the name of the currently executing function, and can be omitted.
  </p>
  <p xmlns:util="util">
    This property allows a function to handle a variable number of arguments. The <b>length</b> property of the <b>arguments</b> object contains the number of arguments passed to the function. The
    individual arguments contained in the <b>arguments</b> object can be accessed in the same way array elements are accessed.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>arguments</b> property:
</p>

```
function ArgTest(arg1, arg2){ var s = ""; s += "The individual arguments are: " for (n = 0; n &lt; arguments.length; n++){ s += ArgTest.arguments[n]; s += " "; } return(s); }
document.write(ArgTest(1, 2, "hello")); //Output: function ArgTest(arg1, arg2){ var s = ""; s += "The individual arguments are: " for (n = 0; n &lt; arguments.length; n++){ s += ArgTest.arguments[n];
s += " "; } return(s); } document.write(ArgTest(1, 2, "hello")); // Output: The individual arguments are: 1 2 hello
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
    <span sdata="link" xmlns:util="util"><a href="5eb79ca9-bbb8-4a42-aaf5-16a93ecb425f.htm">arguments Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="cc9cfd43-1305-41c8-ad67-545d20f4fafe.htm">function Statement (JavaScript)</a></span>
  </div>
</div>

