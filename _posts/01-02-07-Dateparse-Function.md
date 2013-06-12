---
title: Date.parse Function (JavaScript)
---

### Introduction 

 Parses a string containing a date, and returns the number of milliseconds between that date and midnight, January 1, 1970.

### Syntax 

```
Date.parse(dateVal )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">dateVal</span> argument is either a string containing a date or a VT_DATE value retrieved from an ActiveX object or other object. For
    information about date strings that the <b>Date.parse</b> function can parse. see <span sdata="link">Formatting Date and Time Strings (Windows Scripting - JScript)</span>.
  </p>
  <p xmlns:util="util">
    The <b>Date.parse</b> function returns an integer value representing the number of milliseconds between midnight, January 1, 1970 and the date supplied in <span class="parameter" sdata=
    "paramReference">dateVal</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>Date.parse</b> function.
</p>

```
var dateString = "November 1, 1997 10:15 AM"; var mSec = Date.parse(dateString); document.write(mSec); // Output: 878404500000
```

<p xmlns:util="util">
  The following example returns the difference between the date provided and 1/1/1970.
</p>

```
var minMilli = 1000 * 60; var hrMilli = minMilli * 60; var dyMilli = hrMilli * 24; var ms = Date.parse(new Date("June 1, 1990")); var days = Math.round(ms / dyMilli); var dateStr = ""; dateStr +=
"There are " + days + " days "; dateStr += "between 01/01/1970 and " + testDate; document.write(dateStr); // Output: There are 7456 days between 01/01/1970 and Fri Jun 1 00:00:00 PDT 1990
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
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
</div>

