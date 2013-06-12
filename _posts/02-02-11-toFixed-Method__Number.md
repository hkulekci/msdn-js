---
title: toFixed Method (Number) (JavaScript)
---

### Introduction 

 Represents a number in fixed-point notation.

### Syntax 

```
numObj .toFixed([fractionDigits ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required A <b>Number</b> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">fractionDigits</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The number of digits after the decimal point. Must be in the range 0 &#8211; 20, inclusive.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns a string representation of a number in fixed-point notation, containing <span class="parameter" sdata="paramReference">fractionDigits</span> digits after the decimal point.
  </p>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">fractionDigits</span> is not supplied or <b>undefined</b>, the default value is zero.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use <b>toFixed</b>.
</p>

```
var num = new Number(123); var fix = num.toFixed(); document.write(fix); document.write("&lt;br/&gt;"); num = new Number(123.456); fix = num.toFixed(5); document.write(fix); // Output: // 123
123.45600
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="76e87c37-cf6c-46cc-bafa-04be1fe3d78d.htm">Number Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7c4a6d84-3c1f-4cc4-a67d-7753e5d4ed66.htm">toExponential Method (Number) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ac13c82f-1038-447a-823f-f755bba535ca.htm">toPrecision Method (Number) (JavaScript)</a></span>
  </div>
</div>

