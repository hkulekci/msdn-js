---
title: toString Method (Date)
---

### Introduction 

 Returns a string representation of a date. The format of the string depends on the locale. For U.S. English (en-us), it is as follows: day of the week month day hour : minute :second time zone year

### Syntax 

```
date .toString()
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">date</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The date to represent as a string.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns the string representation of the date.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>toString</b> method with a date.
</p>

```
var myDate = new Date(); myDate.setFullYear(2100, 5, 5); var dateString = myDate.toString(); document.write(dateString); // Output: &lt;date&gt;
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

