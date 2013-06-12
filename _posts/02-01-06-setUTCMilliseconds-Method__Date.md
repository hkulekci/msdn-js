---
title: setUTCMilliseconds Method (Date) (JavaScript)
---

### Introduction 

 Sets the milliseconds value in the Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .setUTCMilliseconds(numMilli )
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">numMilli</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value equal to the millisecond value.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    To set the milliseconds using local time, use the <b>setMilliseconds</b> method.
  </p>
  <p xmlns:util="util">
    If the value of <span class="parameter" sdata="paramReference">numMilli</span> is greater than 999, or is a negative number, the stored number of seconds (and minutes, hours, and so forth, if
    necessary) is incremented an appropriate amount.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setUTCMilliseconds</b> method.
</p>

```
function SetUTCMSecDemo(nmsec){ // Create Date object. var d = new Date(); // Set UTC milliseconds. d.setUTCMilliseconds(nmsec); var s = "Current setting is "; s += d.toUTCString(); s += " and " +
d.getUTCMilliseconds(); s += " milliseconds" return(s); }
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
    <span sdata="link" xmlns:util="util"><a href="1b512146-1e8a-44a4-89da-6cc5338d15cb.htm">getMilliseconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7491d387-7b6a-40df-89e5-55c64795ef70.htm">getUTCMilliseconds Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="6c398961-130e-4f60-802f-6c30e1ef4de4.htm">setMilliseconds Method (Date) (JavaScript)</a></span>
  </div>
</div>

