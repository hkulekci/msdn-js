---
title: constructor Property (Number)
isChild: false
---

## constructor Property (Number) {constructor_property_number_title}

### Introduction 

 Specifies the function that creates a Number.

### Syntax 

```
number .constructor
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">number</span> is the name of a string.
  </p>
  <p xmlns:util="util">
    The <b>constructor</b> property is a member of the prototype of every object that has a prototype. This includes all intrinsic JavaScript objects except the <b>Global</b> and <b>Math</b> objects.
    The <b>constructor</b> property contains a reference to the function that constructs instances of that particular object.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the constructor property.
</p>

```
var num = new Number(); if (num.constructor == Number) document.write("Object is a Number."); else document.write("Object is not a Number."); // Output: // Object is a Number.
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

