---
title: getSeconds Method (Date) (JavaScript)
isChild: false
---

## getSeconds Method (Date) (JavaScript) {getseconds_method_date_javascript_title}

### Introduction 

 Gets the seconds of a Date object, using local time.

### Syntax 

```
dateObj .getSeconds()
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
    Returns an integer between 0 and 59. Zero is returned when the time is less than one second into the current minute. If a <b>Date</b> object was created without specifying the time, by default
    the seconds value is 0.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the seconds value using Universal Coordinated Time (UTC), use the <b>getUTCSeconds</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>getSeconds</b> method.
</p>

```
var date = new Date("1/1/2001"); document.write(date.getSeconds()); document.write("&lt;br/&gt;"); date.setSeconds(5); document.write(date.getSeconds()); // Output: // 0 // 5
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
    <span sdata="link" xmlns:util="util"><a href="2d8ea7dc-79f8-4a9b-b2ab-732db2bcd5fd.htm">getUTCSeconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="986ffa54-1db6-4af2-ab8b-8353f64f0b57.htm">setSeconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e035e282-b39d-4d1d-8771-c17542fd6493.htm">setUTCSeconds Method (Date) (JavaScript)</a></span>
  </div>
</div>

