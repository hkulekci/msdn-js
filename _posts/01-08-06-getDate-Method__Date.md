---
title: getDate Method (Date) (JavaScript)
---

### Introduction 

 Gets the day-of-the-month, using local time.

### Syntax 

```
dateObj .getDate()
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">dateObj</span> reference is a <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    An integer between 1 and 31 that represents the day-of-the-month.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the day-of-the-month using Universal Coordinated Time (UTC), use the <b>getUTCDate</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>getDate</b> method.
</p>

```
var date = new Date("Jan 01, 2001"); var str = "Today's date is: "; str += (date.getMonth() + 1) + "/"; str += date.getDate() + "/"; str += date.getFullYear(); document.write(str); // Output: Today's
date is: 1/1/2001
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <span class="label">Applies To</span>: <span sdata="link"><a href="ce2202bb-7ec9-4f5a-bf48-3a04feff283e.htm">Date Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="9e4c763f-c94c-44c9-9684-cb632d75b62e.htm">getUTCDate Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="a84b9b01-a6d0-489f-8a13-e7af9e9630b2.htm">setDate Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e6c3b876-70fe-4103-b197-6c84c078ce10.htm">setUTCDate Method (Date) (JavaScript)</a></span>
  </div>
</div>

