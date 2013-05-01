## [setFullYear Method (Date) (JavaScript)](setFullYear-Method__Date.html)

### Introduction 

 Sets the year of the Date object using local time.

### Syntax 

```
dateObj .setFullYear(numYear [, numMonth [, numDate ]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">dateObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any <b>Date</b> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numYear</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value for the year.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numMonth</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A zero-based numeric value for the month (0 for January, 11 for December). Must be specified if <span class="parameter" sdata="paramReference">numDate</span> is specified.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numDate</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A numeric value equal for the day of the month.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    All <b>set</b> methods taking optional arguments use the value returned from corresponding <b>get</b> methods, if you do not specify the optional argument. For example, if the <span class=
    "parameter" sdata="paramReference">numMonth</span> argument is optional, but not specified, JavaScript uses the value returned from the <b>getMonth</b> method.
  </p>
  <p xmlns:util="util">
    In addition, if the value of an argument is greater than its calendar range or is negative, the date rolls forward or backward as appropriate.
  </p>
  <p xmlns:util="util">
    To set the year using Universal Coordinated Time (UTC), use the <b>setUTCFullYear</b> method.
  </p>
  <p xmlns:util="util">
    The range of years supported in the date object is approximately 285,616 years before and after 1970.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setFullYear</b> method:
</p>

```
var date1 = new Date("1/1/2001"); date1.setFullYear(2007); var date2 = new Date("1/1/2001"); date2.setFullYear(2008, 10, 3); document.write (date1.toLocaleString()); document.write ("&lt;br /&gt;");
document.write (date2.toLocaleString()); // Output: // Monday, January 01, 2007 12:00:00 AM // Monday, November 03, 2008 12:00:00 AM
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
    <span sdata="link" xmlns:util="util"><a href="e6c51b49-0149-4f9a-aa74-c73c0306f98e.htm">setUTCFullYear Method (Date) (JavaScript)</a></span>
  </div>
</div>

