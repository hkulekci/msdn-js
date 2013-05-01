## [getUTCHours Method (Date) (JavaScript)](getUTCHours-Method__Date.html)

### Introduction 

 Gets the hours value in a Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .getUTCHours()
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
    Returns an integer between 0 and 23 indicating the number of hours since midnight. Zero is returned if the time is before 1:00:00 am. If a <b>Date</b> object was created without specifying the
    time, by default the hour is 0 in UTC time. This time may be non-zero in other time zones.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To get the number of hours elapsed since midnight using local time, use the <b>getHours</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>getUTCHours</b> method.
</p>

```
var date = new Date("1/1/2001"); document.write(date.getUTCHours()); document.write("&lt;br/&gt;"); var date2 = new Date("1/1/2001 11:22:33"); document.write(datee.getUTCHours()); // Output (in the
PST time zone): // 8 // 19
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
    <span sdata="link" xmlns:util="util"><a href="c3936496-a213-4d15-b308-d53926ed310c.htm">getHours Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="460f742d-f8d2-4874-9d07-2fb969fef066.htm">setHours Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="257e36fd-fb06-4a4d-8634-d66a020a1511.htm">setUTCHours Method (Date) (JavaScript)</a></span>
  </div>
</div>

