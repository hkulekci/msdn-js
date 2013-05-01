## [constructor Property (Array)](constructor-Property__Array.html)

### Introduction 

 Specifies the function that creates an array.

### Syntax 

```
array .constructor
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">array</span> is the name of an array.
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
var x = new Array(); if (x.constructor == Array) document.write("Object is an Array."); else document.write("Object is not an Array."); // Output: // Object is an Array.
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

