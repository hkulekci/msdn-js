---
title: setMinutes Method (Date) (JavaScript)
---

### Introduction 

 Sets the minutes value in the Date object using local time.

### Syntax 

```
dateObj .setMinutes(numMinutes [, numSeconds [, numMilli ]])
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
        Optional. A numeric value equal to the seconds value. Must be supplied if the <span class="parameter" sdata="paramReference">numMilli</span> argument is used.
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
    argument not specified, JavaScript uses the value returned from the <b>getSeconds</b> method.
  </p>
  <p xmlns:util="util">
    To set the minutes value using Universal Coordinated Time (UTC), use the <b>setUTCMinutes</b> method.
  </p>
  <p xmlns:util="util">
    If the value of an argument is greater than its range or is a negative number, other stored values are modified accordingly. For example, if the stored date is "Jan 5, 1996 00:00:00" and
    <b>setMinutes(90)</b> is called, the date is changed to "Jan 5, 1996 01:30:00." Negative numbers have a similar behavior.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setMinutes</b> method.
</p>

```
function SetMinutesDemo(nmin, nsec){ var d, s; // Declare variables. d = new Date(); // Create Date object. d.setMinutes( nmin, nsec) ; // Set minutes. s = "Current setting is " + d.toLocaleString()
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
    <span sdata="link" xmlns:util="util"><a href="d4139b5d-04e1-474c-9a83-e9d40597243a.htm">getMinutes Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="b6d92543-b285-4e46-8f47-bba36e53fabd.htm">getUTCMinutes Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="2415e788-6d28-46dd-a103-0931a1fd1446.htm">setUTCMinutes Method (Date) (JavaScript)</a></span>
  </div>
</div>

