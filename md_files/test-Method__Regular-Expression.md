---
title: test Method (Regular Expression) (JavaScript)
isChild: false
---

## test Method (Regular Expression) (JavaScript) {test_method_regular_expression_javascript_title}

### Introduction 

 Returns a Boolean value that indicates whether or not a pattern exists in a searched string.

### Syntax 

```
rgExp .test(str )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">rgExp</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An instance of a <b>Regular Expression</b> object containing the regular expression pattern and applicable flags.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">str</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The string on which to perform the search.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>test</b> method checks to see if a pattern exists within a string and returns <b>true</b> if so, and <b>false</b> otherwise.
  </p>
  <p xmlns:util="util">
    The properties of the global <b>RegExp</b> object are not modified by the <b>test</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>test</b> method. To use this example, pass the function a regular expression pattern and a string. The function will test for the occurrence of
  the regular expression pattern in the string and return a string indicating the results of that search:
</p>

```
function TestDemo(re, teststring) { // Test string for existence of regular expression. var found = re.test(teststring) // Format the output. var s = ""; s += "'" + teststring + "'" if (found) s += "
contains "; else s += " does not contain "; s += "'" + re.source + "'" return(s); }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="346aa83e-a045-47ea-acae-b42c7b121534.htm">Regular Expression Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7f6b1073-8cbb-49ed-94b6-56833ba663c5.htm">RegExp Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="346aa83e-a045-47ea-acae-b42c7b121534.htm">Regular Expression Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
</div>

