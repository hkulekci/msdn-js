---
title: valueOf Method (Date)
isChild: false
---

## valueOf Method (Date) {valueof_method_date_title}

### Introduction 

 Returns the stored time value in milliseconds since midnight, January 1, 1970 UTC.

### Syntax 

```
date .valueOf()
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">date</span> object is any instance of a Date.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The stored time value in milliseconds since midnight, January 1, 1970 UTC. This is the same value as <b>getTime</b>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>valueOf</b> method with a date.
</p>

```
var myDate = new Date(); myDate.setFullYear(2100, 5, 5); if (myDate.getTime() == myDate.valueOf()) document.write("values are the same"); else document.write("values are different"); // Output:
values are the same
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

