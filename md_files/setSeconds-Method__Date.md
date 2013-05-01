## [setSeconds Method (Date) (JavaScript)](setSeconds-Method__Date.html)

### Introduction 

 Sets the seconds value in the Date object using local time.

### Syntax 

```
dateObj .setSeconds(numSeconds [, numMilli ])
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
      <i xmlns:util="util">numSeconds</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value equal to the seconds value.
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
    "parameter" sdata="paramReference">numMilli</span> argument is not specified, JavaScript uses the value returned from the <b>getMilliseconds</b> method.
  </p>
  <p xmlns:util="util">
    To set the seconds value using Universal Coordinated Time (UTC), use the <b>setUTCSeconds</b> method.
  </p>
  <p xmlns:util="util">
    If the value of an argument is greater than its range or is a negative number, other stored values are modified accordingly. For example, if the stored date is "Jan 5, 1996 00:00:00" and
    <b>setSeconds(150)</b> is called, the date is changed to "Jan 5, 1996 00:02:30."
  </p>
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="setHours"><span class="keyword">setHours</span></span> method can be used to set the hours, minutes, seconds, and milliseconds.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setSeconds</b> method.
</p>

```
function SetSecondsDemo(nsec){ var d = new Date(); //Create Date object. d.setSeconds( nsec) ; //Set seconds. var s = "Current setting is "; s += d.toLocaleString(); return(s); //Return new setting.
}
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
    <span sdata="link" xmlns:util="util"><a href="97b10674-af0b-4681-a846-38f972196501.htm">getSeconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="2d8ea7dc-79f8-4a9b-b2ab-732db2bcd5fd.htm">getUTCSeconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e035e282-b39d-4d1d-8771-c17542fd6493.htm">setUTCSeconds Method (Date) (JavaScript)</a></span>
  </div>
</div>

