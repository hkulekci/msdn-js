---
title: Math.log Function (JavaScript)
isChild: false
---

## Math.log Function (JavaScript) {mathlog_function_javascript_title}

### Introduction 

 Returns the natural logarithm (base e ) of a number.

### Syntax 

```
Math.log(number )
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <dl class="authored">
    <dt>
      number
    </dt>
    <dd>
      <p xmlns:util="util">
        A number.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">number</span> is positive, this function returns the natural logarithm of the number. If <span class="parameter" sdata=
    "paramReference">number</span> is negative, this function returns <span sdata="langKeyword" value="NaN"><span class="keyword">NaN</span></span>. If <span class="parameter" sdata=
    "paramReference">number</span> is 0, this function returns <span sdata="langKeyword" value="-Infinity"><span class="keyword">-Infinity</span></span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use this function.
</p>

```
var numArr = [ 45.3, 69.0, 557.04, 0.222 ]; for (i in numArr) { document.write(Math.log(numArr[i])); document.write("&lt;br/&gt;"); } // Output: // 3.8133070324889884 // 4.23410650459726 //
6.322637050634291 // -1.5050778971098575
```

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
    <span sdata="link" xmlns:util="util"><a href="6c5438f5-ab03-4e50-969e-1da2330afc04.htm">Math.sqrt Function (JavaScript)</a></span>
  </div>
</div>

