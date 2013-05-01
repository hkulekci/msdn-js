## [typeof Operator (JavaScript)](typeof-Operator.html)

### Introduction 

 Returns a string that identifies the data type of an expression.

### Syntax 

```
typeof[(]expression [)] ;
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <i>expression</i> argument is any expression for which type information is sought.
  </p>
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="typeof"><span class="keyword">typeof</span></span> operator returns type information as a string. There are six possible values that <span sdata="langKeyword"
    value="typeof"><span class="keyword">typeof</span></span> returns: "number," "string," "boolean," "object," "function," and "undefined."
  </p>
  <p xmlns:util="util">
    The parentheses are optional in the <span sdata="langKeyword" value="typeof"><span class="keyword">typeof</span></span> syntax.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example tests the data type of variables.
</p>

```
var index = 5; var result = (typeof index === 'number'); // Output: true var description = "abc"; var result = (typeof description === 'string'); // Output: true
```

<p xmlns:util="util">
  The following example tests for a data type of <span sdata="langKeyword" value="undefined"><span class="keyword">undefined</span></span> for declared and undeclared variables.
</p>

```
var declared; var result = (declared === undefined); // Output: true var result = (typeof declared === 'undefined'); // Output: true var result = (typeof notDeclared === 'undefined') // Output: true
var obj = {}; var result = (typeof obj.propNotDeclared === 'undefined'); // Output: true // An undeclared variable cannot be compared to undefined, // so the next line generates an error. // var
result = (notDeclared === undefined);
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
    <span sdata="link" xmlns:util="util"><a href="58f7d2e0-d310-4292-b9bc-37a73c585780.htm">Array.isArray Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1c59cd7a-a7e2-4c5c-83ec-e6bd2b104d9f.htm">Object.getPrototypeOf Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="2a689d7d-00b0-48fb-9c95-5c2867bde006.htm">undefined Constant (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="084f90f0-d010-47cf-96dd-13d637fc9b68.htm">Comparison Operators (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Data Types (Windows Scripting - JScript)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

