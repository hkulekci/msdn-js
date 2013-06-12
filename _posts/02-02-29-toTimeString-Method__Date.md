---
title: toTimeString Method (Date) (JavaScript)
---

### Introduction 

 Returns a time as a string value.

### Syntax 

```
objDate . toTimeString( )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">objDate</span> reference is a <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
  </p>
  <p xmlns:util="util">
    The <b>toTimeString</b> method returns a string value containing the time in the current time zone.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  In the following example, the time is set to 2000 milliseconds after midnight January 1, 1970 UTC, and then it is written out.
</p>

```
var aDate = new Date(); aDate.setTime(2000); document.write(aDate.toTimeString()); // Output depends on the time in the current time zone.
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
    <span sdata="link" xmlns:util="util"><a href="87d713aa-fd55-4f90-9a30-6df8abdfebe0.htm">toDateString Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8ad75bf5-864c-4a2a-be90-220e87dce172.htm">toLocaleTimeString Method (Date) (JavaScript)</a></span>
  </div>
</div>

