---
title: setUTCFullYear Method (Date) (JavaScript)
---

### Introduction 

 Sets the year value in the Date object using Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .setUTCFullYear(numYear [, numMonth [, numDate ]])
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">numYear</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value equal to the year.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numMonth</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A numeric value equal to the month. The value for January is 0, and other month values follow consecutively. Must be supplied if <i>numDate</i> is supplied.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">numDate</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A numeric value equal to the day of the month.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    All <b>set</b> methods taking optional arguments use the value returned from corresponding <b>get</b> methods, if you do not specify an optional argument. For example, if the <span class=
    "parameter" sdata="paramReference">numMonth</span> argument is not specified, JavaScript uses the value returned from the <b>getUTCMonth</b> method.
  </p>
  <p xmlns:util="util">
    In addition, if the value of an argument is greater that its range or is a negative number, other stored values are modified accordingly.
  </p>
  <p xmlns:util="util">
    To set the year using local time, use the <b>setFullYear</b> method.
  </p>
  <p xmlns:util="util">
    The range of years supported in the <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object is approximately 285,616 years from either side of 1970.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setUTCFullYear</b> method.
</p>

```
var dtFirst = new Date(); dtFirst.setUTCFullYear(2007); var dtSecond = new Date(); // 10 is the value for November. dtSecond.setUTCFullYear(2008, 10, 3); document.write (dtFirst.toUTCString());
document.write ("&lt;br /&gt;"); document.write (dtSecond.toUTCString());
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
    <span sdata="link" xmlns:util="util"><a href="f9ec1262-02e9-4791-90b5-48f33b1dc4bc.htm">getFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="f11e5363-ef8a-48dd-9d56-4ee7290c7c48.htm">getUTCFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="635e4f5a-0210-4c01-8152-b0da4146f6ff.htm">setFullYear Method (Date) (JavaScript)</a></span>
  </div>
</div>

