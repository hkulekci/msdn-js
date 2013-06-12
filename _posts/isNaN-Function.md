---
title: isNaN Function (JavaScript)
isChild: false
---

## isNaN Function (JavaScript) {isnan_function_javascript_title}

### Introduction 

 Returns a Boolean value that indicates whether a value is the reserved value NaN (not a number).

### Syntax 

```
isNaN(numValue )
```

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if the value converted to the <span sdata="langKeyword" value="Number"><span class="keyword">Number</span></span>
    type is the <span sdata="langKeyword" value="NaN"><span class="keyword">NaN</span></span>, otherwise <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">numValue</span> is the value to be tested against <b>NaN</b>.
  </p>
  <p xmlns:util="util">
    You typically use this method to test return values from the <b>parseInt</b> and <b>parseFloat</b> methods.
  </p>
  <p xmlns:util="util">
    Alternatively, a variable that contains <b>NaN</b> or another value could be compared to itself. If it compares as unequal, it is <b>NaN</b>. This is because <b>NaN</b> is the only value that is
    not equal to itself.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="81a40cad-9354-4e38-8ad0-83fc4257baee.htm">Global Object (JavaScript)</a></span>
  </p>
</div>

#### Example 

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ea9287d2-892f-496b-86b7-f9196868d5cf.htm">isFinite Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d57d52ab-81e2-42a5-9360-99a489eb9406.htm">NaN Constant (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="a7d87a69-1919-4623-be85-972e6376dd2d.htm">parseFloat Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e86471af-2a0e-4359-83af-f1ac81e51421.htm">parseInt Function (JavaScript)</a></span>
  </div>
</div>

