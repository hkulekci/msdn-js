## [setUTCDate Method (Date) (JavaScript)](setUTCDate-Method__Date.html)

### Introduction 

 Sets the numeric day of the month in the Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .setUTCDate(numDate )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">dateObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">numDate</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value equal to the day of the month.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To set the day of the month using local time, use the <b>setDate</b> method.
  </p>
  <p xmlns:util="util">
    If the value of <i>numDate</i> is greater than the number of days in the month stored in the <b>Date</b> object or is a negative number, the date is set to a date equal to <i>numDate</i> minus
    the number of days in the stored month. For example, if the stored date is January 5, 1996, and <b>setUTCDate(32)</b> is called, the date changes to February 1, 1996. Negative numbers have a
    similar behavior.
  </p>
  <p xmlns:util="util">
    The <b>setUTCFullYear</b> method can be used to set the year, month, and day of the month.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setUTCDate</b> method.
</p>

```
function SetUTCDateDemo(newdayofmonth){ var d = new Date(); // Create Date object. d.setUTCDate( newdayofmonth) ; // Set UTC day of month. var s = "Current setting is "; s += d.toUTCString();
return(s); // Return new setting. }
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
    <span sdata="link" xmlns:util="util"><a href="67e7f07c-dd46-4b42-82d6-e53e4bd33703.htm">getDate Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="9e4c763f-c94c-44c9-9684-cb632d75b62e.htm">getUTCDate Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="a84b9b01-a6d0-489f-8a13-e7af9e9630b2.htm">setDate Method (Date) (JavaScript)</a></span>
  </div>
</div>

