---
title: toUTCString Method (Date) (JavaScript)
---

### Introduction 

 Returns a date converted to a string using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .toUTCString()
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">dateObj</span> reference is any <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
  </p>
  <p xmlns:util="util">
    The <b>toUTCString</b> method returns a <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object that contains the date formatted using UTC convention in a
    convenient, easily read form.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>toUTCString</b> method.
</p>

```
function toUTCStrDemo(){ var d, s; //Declare variables. d = new Date(); //Create Date object. s = "Current setting is "; s += d.toUTCString() ; //Convert to UTC string. return(s); //Return UTC
string. }
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
    <span sdata="link" xmlns:util="util"><a href="9dc1e722-5722-4b8c-a213-a2650f55f207.htm">toGMTString Method (Date) (JavaScript)</a></span>
  </div>
</div>

