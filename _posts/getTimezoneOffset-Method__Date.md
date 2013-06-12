---
title: getTimezoneOffset Method (Date) (JavaScript)
isChild: false
---

## getTimezoneOffset Method (Date) (JavaScript) {gettimezoneoffset_method_date_javascript_title}

### Introduction 

 Gets the difference in minutes between the time on the local computer and Universal Coordinated Time (UTC).

### Syntax 

```
dateObj .getTimezoneOffset()
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">dateObj</span> reference is a <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns the number of minutes between the time on the current computer (either the client machine or, if this method is called from a server script, the server machine) and UTC. It is positive if
    the current computer's local time is behind UTC (e.g., Pacific Daylight Time), and negative if the current computer's local time is ahead of UTC (e.g., Japan). If a server in New York City is
    contacted by a client in Los Angeles on December 1, <b>getTimezoneOffset</b> returns 480 if executed on the client, or 300 if executed on the server.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>getTimezoneOffset</b> method.
</p>

```
var date = new Date(); var minutes = date.getTimezoneOffset(); if (minutes &lt; 0) document.write(minutes / 60 + " hours after UTC"); else document.write(minutes / 60 + " hours before UTC"); //
Output (for example, where local time is PST): 7 hours before UTC
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

