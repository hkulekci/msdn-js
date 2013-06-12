---
title: setMonth Method (Date) (JavaScript)
---

### Introduction 

 Sets the month value in the Date object using local time.

### Syntax 

```
dateObj . setMonth(numMonth [, dateVal ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">dateObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any <b>Date</b> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numMonth</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value equal to the month. The value for January is 0, and other month values follow consecutively.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">dateVal</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A numeric value representing the day of the month. If this value is not supplied, the value from a call to the <b>getDate</b> method is used.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To set the month value using Universal Coordinated Time (UTC), use the <b>setUTCMonth</b> method.
  </p>
  <p xmlns:util="util">
    If the value of <span class="parameter" sdata="paramReference">numMonth</span> is greater than 11 (January is month 0) or is a negative number, the stored year is modified accordingly. For
    example, if the stored date is "Jan 5, 1996" and <b>setMonth(14)</b> is called, the date is changed to "Mar 5, 1997."
  </p>
  <p xmlns:util="util">
    The <b>setFullYear</b> method can be used to set the year, month, and day of the month.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setMonth</b> method.
</p>

```
date = new Date('1/1/1990'); date.setMonth(14); document.write(date); // Output: Fri Mar 1 00:00:00 PST 1991 // Note that the time zone corresponds to the time zone on the local computer.
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
    <span sdata="link" xmlns:util="util"><a href="eabae139-4da0-4e4a-a4cb-608e6375fc9e.htm">getUTCMonth Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="cdac5f64-c4fd-44cc-ba3a-9a8dd3dd3fad.htm">setUTCMonth Method (Date) (JavaScript)</a></span>
  </div>
</div>

