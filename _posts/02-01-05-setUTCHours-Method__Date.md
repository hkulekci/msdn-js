---
title: setUTCHours Method (Date) (JavaScript)
---

### Introduction 

 Sets the hours value in the Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .setUTCHours(numHours [, numMin [, numSec [, numMilli ]]])
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">numHours</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value equal to the hours value.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numMin</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A numeric value equal to the minutes value. Must be supplied if either <span class="parameter" sdata="paramReference">numSec</span> or <span class="parameter" sdata=
        "paramReference">numMilli</span> are used.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numSec</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A numeric value equal to the seconds value. Must be supplied if <span class="parameter" sdata="paramReference">numMilli</span> argument is used.
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
    All <b>set</b> methods taking optional arguments use the value returned from corresponding <b>get</b> methods, if you do not specify an optional argument. For example, if the <span class=
    "parameter" sdata="paramReference">numMin</span> argument is not specified, JavaScript uses the value returned from the <b>getUTCMinutes</b> method.
  </p>
  <p xmlns:util="util">
    To set the hours value using local time, use the <b>setHours</b> method.
  </p>
  <p xmlns:util="util">
    If the value of an argument is greater than its range, or is a negative number, other stored values are modified accordingly. For example, if the stored date is "Jan 5, 1996 00:00:00.00", and
    <b>setUTCHours(30)</b> is called, the date is changed to "Jan 6, 1996 06:00:00.00."
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setUTCHours</b> method.
</p>

```
function SetUTCHoursDemo(nhr, nmin, nsec){ var d, s; // Declare variables. d = new Date(); // Create Date object. d.setUTCHours( nhr, nmin, nsec) ; // Set UTC hours, minutes, seconds. s = "Current
setting is " + d.toUTCString() return(s); // Return new setting. }
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
    <span sdata="link" xmlns:util="util"><a href="7c9825dd-4b3a-4614-8e09-f40df123b630.htm">getUTCHours Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="460f742d-f8d2-4874-9d07-2fb969fef066.htm">setHours Method (Date) (JavaScript)</a></span>
  </div>
</div>

