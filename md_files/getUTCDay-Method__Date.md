---
title: getUTCDay Method (Date) (JavaScript)
isChild: false
---

## getUTCDay Method (Date) (JavaScript) {getutcday_method_date_javascript_title}

### Introduction 

 Gets the day of the week using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .getUTCDay()
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
    Returns an integer between 0 (Sunday) and 6 (Saturday) that represents the day of the week.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the day of the week using local time, use the <b>getDate</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>getUTCDay</b> method.
</p>

```
var date = new Date("2/6/2001"); var day = date.getUTCDay(); document.write(day); // Output: 2
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
    <span sdata="link" xmlns:util="util"><a href="27be7168-3dce-41c9-ae69-6280b7984c2e.htm">getDay Method (Date) (JavaScript)</a></span>
  </div>
</div>

