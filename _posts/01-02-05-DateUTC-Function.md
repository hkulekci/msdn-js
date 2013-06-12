---
title: Date.UTC Function (JavaScript)
---

### Introduction 

 Returns the number of milliseconds between midnight, January 1, 1970 Universal Coordinated Time (UTC) (or GMT) and the specified date.

### Syntax 

```
Date.UTC(year , month , day [, hours [, minutes [, seconds [,ms ]]]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">year</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The full year designation is required for cross-century date accuracy. If <span class="parameter" sdata="paramReference">year</span> is between 0 and 99 is used, then <span class=
        "parameter" sdata="paramReference">year</span> is assumed to be 1900 + <span class="parameter" sdata="paramReference">year</span>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">month</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The month as an integer between 0 and 11 (January to December).
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">day</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The date as an integer between 1 and 31.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">hours</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Must be supplied if <span class="parameter" sdata="paramReference">minutes</span> is supplied. An integer from 0 to 23 (midnight to 11pm) that specifies the hour.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">minutes</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Must be supplied if <span class="parameter" sdata="paramReference">seconds</span> is supplied. An integer from 0 to 59 that specifies the minutes.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">seconds</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Must be supplied if <span class="parameter" sdata="paramReference">milliseconds</span> is supplied. An integer from 0 to 59 that specifies the seconds.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">ms</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. An integer from 0 to 999 that specifies the milliseconds.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Date.UTC</b> function returns the number of milliseconds between midnight, January 1, 1970 UTC and the supplied date. This return value can be used in the <b>setTime</b> method and in the
    <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object constructor. If the value of an argument is greater than its range, or is a negative number, other stored
    values are modified accordingly. For example, if you specify 150 seconds, JavaScript redefines that number as two minutes and 30 seconds.
  </p>
  <p xmlns:util="util">
    The difference between the <b>Date.UTC</b> function and the <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object constructor that accepts a date is that the
    <b>Date.UTC</b> function assumes UTC, and the <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object constructor assumes local time.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>Date.UTC</b> function.
</p>

```
// Determine the milliseconds per day. var MinMilli = 1000 * 60; var HrMilli = MinMilli * 60; var DyMilli = HrMilli * 24; var date = new Date("June 1, 1990"); var year = date.getFullYear(); var month
= date.getMonth(); var day = date.getDay(); var newDay = new Date("January 16, 2020"); var yeartoday = newDay.getUTCFullYear(); var monthtoday = newDay.getUTCMonth(); var dayofmonthtoday =
newDay.getUTCDate(); // Get the milliseconds since 1/1/1970 UTC. var t1 = Date.UTC(year, month - 1, day) var t2 = Date.UTC(yeartoday, monthtoday, dayofmonthtoday); // Determine the difference in
days. var days = (t2 - t1) / DyMilli; document.write(days); // Output: 10848
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
    <span sdata="link" xmlns:util="util"><a href="86584748-7219-495b-bf56-e27f5782778c.htm">setTime Method (Date) (JavaScript)</a></span>
  </div>
</div>

