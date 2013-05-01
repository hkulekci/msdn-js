## [Debug.writeln Function (JavaScript)](Debug.writeln-Function.html)

### Introduction 

 Sends strings to the script debugger, followed by a newline character.

### Syntax 

```
Debug.writeln([str1 [, str2 [, ... [, strN ]]]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">str1, str2, ... , strN</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Strings to send to the script debugger.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Debug.writeln</b> function sends strings, followed by a newline character, to the Immediate window of the Microsoft Script Debugger at run time. If the script is not being debugged, the
    <b>Debug.writeln</b> function has no effect.
  </p>
  <p xmlns:util="util">
    The <b>Debug.writeln</b> function is almost identical to the <b>Debug.write</b> function. The only difference is that the <b>Debug.write</b> function does not send a newline character after
    sending the strings.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  This example uses the <b>Debug.writeln</b> function to display the value of the variable in the Immediate window of the Microsoft Script Debugger.
</p>

```
var counter = 42; Debug.writeln( "The value of counter is " + counter) ;
```

<p xmlns:util="util">
  To run this example, you must have a script debugger installed and the script must run in debug mode.
</p>

```
<p xmlns:util="util">
  To run this example, you must have a script debugger installed and the script must run in debug mode.
</p>
```

<p xmlns:util="util">
  Internet Explorer 8 includes the JavaScript debugger. If you are using an earlier version of Internet Explorer, see <a href="http://go.microsoft.com/fwlink/?LinkId=133801">How to: Enable and Start
  Script Debugging from Internet Explorer</a>.
</p>

```
<p xmlns:util="util">
  Internet Explorer 8 includes the JavaScript debugger. If you are using an earlier version of Internet Explorer, see <a href="http://go.microsoft.com/fwlink/?LinkId=133801">How to: Enable and Start
  Script Debugging from Internet Explorer</a>.
</p>
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="42a367ec-beb1-4e59-8342-34c326eca042.htm">Debug Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="fd1cfbb3-46cb-47cc-896c-a70d457dd413.htm">Debug.write Function (JavaScript)</a></span>
  </div>
</div>

