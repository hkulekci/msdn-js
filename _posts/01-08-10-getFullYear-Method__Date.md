---
title: getFullYear Method (Date) (JavaScript)
---

### Introduction 

 Gets the year, using local time.

### Syntax 

```
dateObj .getFullYear()
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
    The year as a four-digit number. For example, the year 1976 is returned as 1976. Years specified as two digits in the <b>Date</b> constructor or in <b>setFullYear</b> are assumed to be in the
    twentieth century, so given "5/14/12", <b>getFullYear</b> returns "1912".
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the year using Universal Coordinated Time (UTC), use the <b>getUTCFullYear</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>getFullYear</b> method.
</p>

```
var date = new Date("1/1/01"); document.write(date.getFullYear()); // Output: 1901
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
    <span sdata="link" xmlns:util="util"><a href="f11e5363-ef8a-48dd-9d56-4ee7290c7c48.htm">getUTCFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="635e4f5a-0210-4c01-8152-b0da4146f6ff.htm">setFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e6c51b49-0149-4f9a-aa74-c73c0306f98e.htm">setUTCFullYear Method (Date) (JavaScript)</a></span>
  </div>
</div>

