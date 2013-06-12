---
title: Debug Object (JavaScript)
---

### Introduction 

 An intrinsic global object that sends output to a debugger.

### Syntax 

```
Debug.function
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You do not instantiate the Debug object. You can access all its properties and methods by calling <span class="parameter" sdata="paramReference">function</span>.
  </p>
  <p xmlns:util="util">
    There are different ways to debug Internet Explorer and Windows Store apps. In Windows Store apps, the <b>write</b> and <b>writeln</b> functions of the <b>Debug</b> object display strings in the
    Visual Studio <span class="ui">Output</span> window at run time. For more information about debugging Windows Store apps, see <span sdata="link">Debugging Windows Metro style apps</span>.
  </p>
  <p xmlns:util="util">
    To debug Internet Explorer scripts, you must have a script debugger installed and the script must run in debug mode. Internet Explorer 8 and later versions include the JavaScript debugger. If you
    are using an earlier version of Internet Explorer, see <a href="http://go.microsoft.com/fwlink/?LinkId=133801">How to: Enable and Start Script Debugging from Internet Explorer</a>.
  </p>
  <p xmlns:util="util">
    If the script is not being debugged, the functions have no effect.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  This example uses the <b>write</b> function to display the value of the variable.
</p>

```
var counter = 42; Debug.write("The value of counter is " + counter);
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

#### Properties 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    <span sdata="link"><a href="8a0b8c10-eda3-4936-8c9f-572760ffcb96.htm">Debug.debuggerEnabled Property</a></span> | <span sdata="link"><a href=
    "1dd2abee-a415-41bb-a359-017da62f9485.htm">Debug.setNonUserCodeExceptions Property</a></span>
  </p>
</div>

#### Functions 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    <span sdata="link"><a href="fd1cfbb3-46cb-47cc-896c-a70d457dd413.htm">Debug.write Function (JavaScript)</a></span> | <span sdata="link"><a href=
    "c3aad0cd-0486-4161-9ba6-31d672da72af.htm">Debug.writeln Function (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="c6d2e193-c1f7-4fb3-8a4e-cc9823174ae4.htm">debugger Statement (JavaScript)</a></span>
  </div>
</div>

