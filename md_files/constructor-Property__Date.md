## [constructor Property (Date)](constructor-Property__Date.html)

### Introduction 

 Specifies the function that creates a date.

### Syntax 

```
date .constructor
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">date</span> is the name of a date object.
  </p>
  <p xmlns:util="util">
    The <b>constructor</b> property is a member of the prototype of every object that has a prototype. The <b>constructor</b> property contains a reference to the function that constructs instances
    of that particular object.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the constructor property.
</p>

```
var x = new Date("Hi"); if (x.constructor == Date) document.write("Object is a date."); // Output: // Object is a date.
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

