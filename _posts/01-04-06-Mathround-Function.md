---
title: Math.round Function (JavaScript)
---

### Introduction 

 Returns a supplied numeric expression rounded to the nearest integer.

### Syntax 

```
Math.round(number )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">number</span> argument is the value to be rounded to the nearest integer.
  </p>
  <p xmlns:util="util">
    For positive numbers, if the decimal portion of <span class="parameter" sdata="paramReference">number</span> is 0.5 or greater, the return value is equal to the smallest integer greater than
    <span class="parameter" sdata="paramReference">number</span>. If the decimal portion is less than 0.5, the return value is the largest integer less than or equal to <span class="parameter" sdata=
    "paramReference">number</span>.
  </p>
  <p xmlns:util="util">
    For negative numbers, if the decimal portion is exactly -0.5, the return value is the smallest integer that is greater than the number.
  </p>
  <p xmlns:util="util">
    For example, <span class="code">Math.round(8.5)</span> returns 9, but <span class="code">Math.round(-8.5)</span> returns -8.
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
    <b>Applies To</b>: <span sdata="link"><a href="607b94cb-921c-43cd-b514-fdbc13aeced6.htm">Math Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="a28c5c66-c42f-4082-9b71-9a5ee4652cd7.htm">Math.random Function (JavaScript)</a></span>
  </div>
</div>

