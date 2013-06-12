---
title: Math.max Function (JavaScript)
isChild: false
---

## Math.max Function (JavaScript) {mathmax_function_javascript_title}

### Introduction 

 Returns the larger of a set of supplied numeric expressions.

### Syntax 

```
Math.max([number1 [, number2 [... [, numberN ]]]])
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The optional <span class="parameter" sdata="paramReference">number1, number2, ..., numberN</span> arguments are numeric expressions to be evaluated.
  </p>
  <p xmlns:util="util">
    If no arguments are provided, the return value is equal to Number.NEGATIVE_INFINITY. If any argument is <b>NaN</b>, the return value is also <b>NaN</b>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to get the larger of two expressions.
</p>

```
var x = Math.max(107 - 3, 48 * 90); document.write(x); // Output: // 4320
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
    <span sdata="link" xmlns:util="util"><a href="a1d7dd85-27ef-45cd-aa2a-f8e80f0b2898.htm">Math.min Function (JavaScript)</a></span>
  </div>
</div>

