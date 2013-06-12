---
title: getUTCMonth Method (Date) (JavaScript)
isChild: false
---

## getUTCMonth Method (Date) (JavaScript) {getutcmonth_method_date_javascript_title}

### Introduction 

 Gets the month of a Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .getUTCMonth()
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
    Returns an integer between 0 (January) and 11 (December).
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the month in local time, use the <b>getMonth</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>getUTCMonth</b> method.
</p>

```
var date = new Date("2/2/2002"); document.write(date.getUTCMonth()); // Output: 1
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
    <span sdata="link" xmlns:util="util"><a href="c20dd8ba-1d78-42f1-8717-ed3dfd2362dd.htm">getMonth Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4f5be295-d536-46c0-b3a4-ad06457efe82.htm">setMonth Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="cdac5f64-c4fd-44cc-ba3a-9a8dd3dd3fad.htm">setUTCMonth Method (Date) (JavaScript)</a></span>
  </div>
</div>

