---
title: charCodeAt Method (String) (JavaScript)
---

### Introduction 

 Returns the Unicode value of the character at the specified location.

### Syntax 

```
strObj . charCodeAt(index )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">strObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">index</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The zero-based index of the desired character. If there is no character at the specified index, <span sdata="langKeyword" value="NaN"><span class="keyword">NaN</span></span> is
        returned.
      </p>
    </dd>
  </dl>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>charCodeAt</b> method.
</p>

```
var str = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"; document.write(str.charCodeAt(str.length - 1)); // Output: 90
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
    <span sdata="link" xmlns:util="util"><a href="f64120c1-23a7-48ca-8d1c-db3e8856cab4.htm">String.fromCharCode Function (JavaScript)</a></span>
  </div>
</div>

