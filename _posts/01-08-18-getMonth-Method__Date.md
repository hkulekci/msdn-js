---
title: getMonth Method (Date) (JavaScript)
---

### Introduction 

 Gets the month, using local time.

### Syntax 

```
dateObj .getMonth()
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
    The <b>getMonth</b> method returns an integer between 0 (January) and 11 (December). For a <b>Date</b> constructed with "Jan 5, 1996", <b>getMonth</b> returns 0.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the month value using Universal Coordinated Time (UTC), use the <b>getUTCMonth</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>getMonth</b> method.
</p>

```
var date = new Date("1/1/2001"); document.write(date.getMonth()); // Output: 0
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
    <span sdata="link" xmlns:util="util"><a href="eabae139-4da0-4e4a-a4cb-608e6375fc9e.htm">getUTCMonth Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4f5be295-d536-46c0-b3a4-ad06457efe82.htm">setMonth Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="cdac5f64-c4fd-44cc-ba3a-9a8dd3dd3fad.htm">setUTCMonth Method (Date) (JavaScript)</a></span>
  </div>
</div>

