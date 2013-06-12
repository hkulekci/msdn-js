---
title: getUTCMilliseconds Method (Date) (JavaScript)
---

### Introduction 

 Gets the milliseconds of a Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .getUTCMilliseconds()
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
    Returns a millisecond value that can range from 0-999.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the number of milliseconds in local time, use the <b>getMilliseconds</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>getUTCMilliseconds</b> method.
</p>

```
var date = new Date("1/1/2001"); document.write(date.getUTCMilliseconds()); document.write("&lt;br/&gt;"); date.setMilliseconds(34); document.writedate.getUTCMilliseconds()); // Output: // 0 // 34
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
    <span sdata="link" xmlns:util="util"><a href="1b512146-1e8a-44a4-89da-6cc5338d15cb.htm">getMilliseconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="6c398961-130e-4f60-802f-6c30e1ef4de4.htm">setMilliseconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ed8e4486-d4b2-4b73-836b-dd1d3bb991a0.htm">setUTCMilliseconds Method (Date) (JavaScript)</a></span>
  </div>
</div>

