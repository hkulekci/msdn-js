---
title: getUTCDate Method (Date) (JavaScript)
isChild: false
---

## getUTCDate Method (Date) (JavaScript) {getutcdate_method_date_javascript_title}

### Introduction 

 Gets the day-of-the-month, using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .getUTCDate()
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
    Returns an integer between 1 and 31 that represents the day-of-the-month.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the day of the month using local time, use the <b>getDate</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>getUTCDate</b> method.
</p>

```
var date = new Date("1/23/2001"); document.write(date.getUTCDate()); // Output: 23
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
    <span sdata="link" xmlns:util="util"><a href="67e7f07c-dd46-4b42-82d6-e53e4bd33703.htm">getDate Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="a84b9b01-a6d0-489f-8a13-e7af9e9630b2.htm">setDate Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e6c3b876-70fe-4103-b197-6c84c078ce10.htm">setUTCDate Method (Date) (JavaScript)</a></span>
  </div>
</div>

