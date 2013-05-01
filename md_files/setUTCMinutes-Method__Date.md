## [setUTCMinutes Method (Date) (JavaScript)](setUTCMinutes-Method__Date.html)

### Introduction 

 Sets the minutes value in the Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .setUTCMinutes(numMinutes [, numSeconds [, numMilli ]])
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">numMinutes</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value equal to the minutes value. Must be supplied if either of the following arguments is used.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">numSeconds</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A numeric value equal to the seconds value. Must be supplied if <span class="parameter" sdata="paramReference">numMilli</span> is used.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numMilli</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A numeric value equal to the milliseconds value.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    All <b>set</b> methods taking optional arguments use the value returned from corresponding <b>get</b> methods, if you do not specify an optional argument. For example, if the <i>numSeconds</i>
    argument is not specified, JavaScript uses the value returned from the <b>getUTCSeconds</b> method.
  </p>
  <p xmlns:util="util">
    To modify the minutes value using local time, use the <b>setMinutes</b> method.
  </p>
  <p xmlns:util="util">
    If the value of an argument is greater than its range, or is a negative number, other stored values are modified accordingly. For example, if the stored date is "Jan 5, 1996 00:00:00.00", and
    <b>setUTCMinutes(70)</b> is called, the date is changed to "Jan 5, 1996 01:10:00.00."
  </p>
  <p xmlns:util="util">
    The <b>setUTCHours</b> method can be used to set the hours, minutes, seconds, and milliseconds.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setUTCMinutes</b> method:
</p>

```
function SetUTCMinutesDemo(nmin, nsec){ var d, s; // Declare variables. d = new Date(); // Create Date object. d.setUTCMinutes( nmin,nsec) ; // Set UTC minutes. s = "Current setting is " +
d.toUTCString() return(s); // Return new setting. }
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
    <span sdata="link" xmlns:util="util"><a href="d4139b5d-04e1-474c-9a83-e9d40597243a.htm">getMinutes Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="b6d92543-b285-4e46-8f47-bba36e53fabd.htm">getUTCMinutes Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="34c959cd-cd29-4cee-8e04-9061cf6d42f3.htm">setMinutes Method (Date) (JavaScript)</a></span>
  </div>
</div>

