## [Math.min Function (JavaScript)](Math.min-Function.html)

### Introduction 

 Returns the smaller of a set of numeric expressions.

### Syntax 

```
Math.min([number1 [, number2 [... [,numberN ]]]])
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The optional <span class="parameter" sdata="paramReference">number1, number2, ..., numberN</span> arguments are numeric expressions to be evaluated.
  </p>
  <p xmlns:util="util">
    If no arguments are provided, the return value is equal to Number.POSITIVE_INFINITY. If any argument is <b>NaN</b>, the return value is also <b>NaN</b>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to get the smaller of two expressions.
</p>

```
var x = Math.min(107 - 3, 48 * 90); document.write(x); // Output: // 104
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
    <span sdata="link" xmlns:util="util"><a href="f3ea1b8a-5fd0-482a-971b-b7f8e2b9b7eb.htm">Math.max Function (JavaScript)</a></span>
  </div>
</div>

