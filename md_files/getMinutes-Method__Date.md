## [getMinutes Method (Date) (JavaScript)](getMinutes-Method__Date.html)

### Introduction 

 Gets the minutes of a Date object, using local time.

### Syntax 

```
dateObj .getMinutes()
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
    Returns an integer between 0 and 59. Zero is returned the time is less than one minute after the hour. If a <b>Date</b> object was created without specifying the time, by default the minute value
    is 0.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the minutes value using Universal Coordinated Time (UTC), use the <b>getUTCMinutes</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to the <b>getMinutes</b> method.
</p>

```
var date = new Date("1/1/2001"); document.write(date.getMinutes()); document.write("&lt;br/&gt;"); date.setMinutes(5); document.write(date.getMinutes()); // Output: // 0 // 5
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
    <span sdata="link" xmlns:util="util"><a href="b6d92543-b285-4e46-8f47-bba36e53fabd.htm">getUTCMinutes Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="34c959cd-cd29-4cee-8e04-9061cf6d42f3.htm">setMinutes Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="2415e788-6d28-46dd-a103-0931a1fd1446.htm">setUTCMinutes Method (Date) (JavaScript)</a></span>
  </div>
</div>

