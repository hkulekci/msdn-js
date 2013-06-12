---
title: toISOString Method (Date) (JavaScript)
---

### Introduction 

 Returns a date as a string value in ISO format.

### Syntax 

```
objDate .toISOString()
```

#### Return Value 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    A string representation of the date in International Organization for Standardization (ISO) format.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">objDate</span> does not contain a valid date, a <span sdata="langKeyword" value="RangeError"><span class="keyword">RangeError</span></span>
    exception is thrown.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The ISO format is a simplification of the ISO 8601 format. For more information, see <span sdata="link">Formatting Date and Time Strings (Windows Scripting - JScript)</span>.
  </p>
  <p xmlns:util="util">
    The time zone is always UTC, denoted by the suffix Z in the output.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>toISOString</b> method.
</p>

```
var dt = new Date("30 July 2010 15:05 UTC"); document.write(dt.toISOString()); document.write("&lt;br /&gt;"); document.write(dt.toUTCString()); // Output: // 2010-07-30T15:05:00.000Z // Fri, 30 Jul
2010 15:05:00 UTC
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Internet Explorer 9 standards and Internet Explorer 10 standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ce2202bb-7ec9-4f5a-bf48-3a04feff283e.htm">Date Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Formatting Date and Time Strings (Windows Scripting - JScript)</span>
  </div>
</div>

