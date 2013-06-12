---
title: eval Function (JavaScript)
---

### Introduction 

 Evaluates JavaScript code and executes it.

### Syntax 

```
eval(codeString )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">codeString</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A <b>String</b> value that contains valid JavaScript code.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>eval</b> function enables dynamic execution of JavaScript source code.
  </p>
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">codeString</span> string is parsed by the JavaScript parser and executed.
  </p>
  <p xmlns:util="util">
    The code passed to the <b>eval</b> function is executed in the same context as the call to the <b>eval</b> function.
  </p>
  <p xmlns:util="util">
    Whenever possible, use the JSON.parse function to de-serialize JavaScript Object Notation (JSON) text. The <b>JSON.parse</b> function is more secure and executes faster than the <b>eval</b>
    function.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code initializes the variable <span class="code">myDate</span> to a test date.
</p>

```
var dateFn = "Date(1971,3,8)"; var myDate; eval("myDate = new " + dateFn + ";"); document.write(myDate); // Output: Thu Apr 8 00:00:00 PDT 1971
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="81a40cad-9354-4e38-8ad0-83fc4257baee.htm">Global Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

