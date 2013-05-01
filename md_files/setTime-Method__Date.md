## [setTime Method (Date) (JavaScript)](setTime-Method__Date.html)

### Introduction 

 Sets the date and time value in the Date object.

### Syntax 

```
dateObj .setTime(milliseconds )
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
      <i xmlns:util="util">milliseconds</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A numeric value representing the number of elapsed milliseconds since midnight, January 1, 1970 GMT.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If <i>milliseconds</i> is negative, it indicates a date before 1970. The range of available dates is approximately 285,616 years from either side of 1970.
  </p>
  <p xmlns:util="util">
    Setting the date and time with the <b>setTime</b> method is independent of the time zone.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>setTime</b> method.
</p>

```
function SetTimeTest(newtime){ var d, s; //Declare variables. d = new Date(); //Create Date object. d.setTime( newtime) ; //Set time. s = "Current setting is "; s += d.toUTCString(); return(s);
//Return new setting. }
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
    <span sdata="link" xmlns:util="util"><a href="f0da1d4e-337c-497d-9205-093defbc6d3d.htm">getTime Method (Date) (JavaScript)</a></span>
  </div>
</div>

