---
title: Array.isArray Function (JavaScript)
---

### Introduction 

 Determines whether an object is an array.

### Syntax 

```
Array.isArray(object )
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The object to test.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if <span class="parameter" sdata="paramReference">object</span> is an array; otherwise, <span sdata="langKeyword"
    value="false"><span class="keyword">false</span></span>. If the <span class="parameter" sdata="paramReference">object</span> argument is not an object, <span sdata="langKeyword" value=
    "false"><span class="keyword">false</span></span> is returned.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>Array.isArray</b> function.
</p>

```
var ar = []; var result = Array.isArray(ar); // Output: true var ar = new Array(); var result = Array.isArray(ar); // Output: true var ar = [1, 2, 3]; var result = Array.isArray(ar); // Output: true
var result = Array.isArray("an array"); document.write(result); // Output: false
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Internet Explorer 9 standards and Internet Explorer 10 standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Using Arrays (Windows Scripting - JScript)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ee8a1036-119f-486f-b034-b07bdba87f0c.htm">typeof Operator (JavaScript)</a></span>
  </div>
</div>

