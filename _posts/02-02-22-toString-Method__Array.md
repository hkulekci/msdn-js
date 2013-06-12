---
title: toString Method (Array)
---

### Introduction 

 Returns a string representation of an array.

### Syntax 

```
array .toString()
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">array</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The array to represent as a string.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The string representation of the array.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The elements of an <b>Array</b> are converted to strings. The resulting strings are concatenated and separated by commas.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>toString</b> method with an array.
</p>

```
var arr = [1, 2, 3, 4]; var s = arr.toString(); document.write(s); // Output: 1,2,3,4
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

