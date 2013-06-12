---
title: toString Method (Error)
---

### Introduction 

 Returns a string representation of an error.

### Syntax 

```
error .toString()
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">date</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The error to represent as a string.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns "Error: " plus the error message.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>toString</b> method with an error.
</p>

```
var myError = new Error(); myError.message = "My Error"; var errorString = myError.toString(); document.write(errorString); // Output: Error: My Error
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

