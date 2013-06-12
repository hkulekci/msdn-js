---
title: getUTCSeconds Method (Date) (JavaScript)
isChild: false
---

## getUTCSeconds Method (Date) (JavaScript) {getutcseconds_method_date_javascript_title}

### Introduction 

 Gets the seconds of a Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .getUTCSeconds()
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">dateObj</span> reference is a <b>Date</b> object.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns an integer between 0 and 59. Zero is returned when the time is less than one second into the current minute. If a <b>Date</b> object was created without specifying the time, by default
    the UTC seconds value is 0.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the number of seconds in local time, use the <b>getSeconds</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>getUTCSeconds</b> method.
</p>

```
var date = new Date("1/1/2001"); document.write(date. getUTCSeconds()); // Output: 0
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="ce2202bb-7ec9-4f5a-bf48-3a04feff283e.htm">Date Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="97b10674-af0b-4681-a846-38f972196501.htm">getSeconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="986ffa54-1db6-4af2-ab8b-8353f64f0b57.htm">setSeconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e035e282-b39d-4d1d-8771-c17542fd6493.htm">setUTCSeconds Method (Date) (JavaScript)</a></span>
  </div>
</div>

