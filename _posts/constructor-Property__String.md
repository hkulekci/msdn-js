---
title: constructor Property (String)
isChild: false
---

## constructor Property (String) {constructor_property_string_title}

### Introduction 

 Specifies the function that creates a string.

### Syntax 

```
string .constructor
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">string</span> is the name of a string.
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
var x = new String(); if (x.constructor == String) document.write("Object is a String."); else document.write("Object is not a String."); // Output: // Object is a String.
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

