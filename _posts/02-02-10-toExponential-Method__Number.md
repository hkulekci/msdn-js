---
title: toExponential Method (Number) (JavaScript)
---

### Introduction 

 Represents a number in exponential notation.

### Syntax 

```
numObj . toExponential([fractionDigits ])
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
    Returns a string representation of a number in exponential notation. The string contains one digit before the decimal point, and may contain <span class="parameter" sdata=
    "paramReference">fractionDigits</span> digits after it.
  </p>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">fractionDigits</span> is not supplied, the <b>toExponential</b> method returns as many digits necessary to uniquely specify the number.
  </p>
</div>

#### Example 

<p xmlns:util="util"></p>

```
var num = new Number(123); var exp = num.toExponential(); document.write(exp); document.write("&lt;br/&gt;"); num = new Number(123.456); exp = num.toExponential(5); document.write(exp); // Output: //
1.23e+2 // 1.23456e+2
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
    <span sdata="link" xmlns:util="util"><a href="ac13c82f-1038-447a-823f-f755bba535ca.htm">toPrecision Method (Number) (JavaScript)</a></span>
  </div>
</div>

