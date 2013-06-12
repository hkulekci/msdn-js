---
title: toPrecision Method (Number) (JavaScript)
isChild: false
---

## toPrecision Method (Number) (JavaScript) {toprecision_method_number_javascript_title}

### Introduction 

 Represents a number either in exponential or fixed-point notation with a specified number of digits.

### Syntax 

```
numObj .toPrecision([precision ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A <b>Number</b> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">precision</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The number of significant digits. Must be in the range 1 &#8211; 21, inclusive.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    For numbers in exponential notation, <span class="parameter" sdata="paramReference">precision</span> - 1 digits are returned after the decimal point. For numbers in fixed notation, <span class=
    "parameter" sdata="paramReference">precision</span> significant digits are returned.
  </p>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">precision</span> is not supplied or is <b>undefined</b>, the <b>toString</b> method is called instead.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use <b>toPrecision</b>.
</p>

```
var num = new Number(123); var prec = num.toPrecision(); document.write(prec); document.write("&lt;br/&gt;"); num = new Number(123.456); prec = num.toPrecision(5); document.write(prec); // Output: //
123 // 123.46
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
    <span sdata="link" xmlns:util="util"><a href="b5f03400-865e-4ab2-818c-f734c0f6d6f0.htm">toFixed Method (Number) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7c4a6d84-3c1f-4cc4-a67d-7753e5d4ed66.htm">toExponential Method (Number) (JavaScript)</a></span>
  </div>
</div>

