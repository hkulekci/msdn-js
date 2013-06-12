---
title: match Method (String) (JavaScript)
isChild: false
---

## match Method (String) (JavaScript) {match_method_string_javascript_title}

### Introduction 

 Matches a string with a regular expression, and returns an array containing the results of that search.

### Syntax 

```
stringObj .match(rgExp )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal on which to perform the search.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">rgExp</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A regular expression object that contains the regular expression pattern and applicable flags. This can also be a variable name or string literal containing the regular expression
        pattern and flags.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the <b>match</b> method does not find a match, it returns <span sdata="langKeyword" value="null"><span class="keyword">null</span></span>. If it finds a match, <b>match</b> returns an array,
    and the properties of the global <b>RegExp</b> object are updated to reflect the results of the match.
  </p>
  <p xmlns:util="util">
    The array returned by the <b>match</b> method has three properties, <b>input</b>, <b>index</b> and <b>lastIndex</b>. The <span class="parameter" sdata="paramReference">input</span> property
    contains the entire searched string. The <span class="parameter" sdata="paramReference">index</span> property contains the position of the matched substring within the complete searched string.
    The <b>lastIndex</b> property contains the position following the last character in the last match.
  </p>
  <p xmlns:util="util">
    If the global flag (<b>g</b>) is not set, Element zero of the array contains the entire match, while elements 1 through <i>n</i> contain any submatches. This behavior is the same as the behavior
    of the <span sdata="link"><a href="83092452-60cc-4218-b4ae-af9e3cb96c34.htm">exec Method (Regular Expression) (JavaScript)</a></span> when the global flag is not set. If the global flag is set,
    elements 0 through <i>n</i> contain all matches that occurred.
  </p>
  <p xmlns:util="util">
    If the flag <b>i</b> is set, the search is not case-sensitive.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="match"><span class="keyword">match</span></span> method.
</p>

```
var src = "azcafAJAC"; var re = /[a-c]/; var result = src.match(re); // The entire match is in array element 0. document.write(result[0] + "&lt;br/&gt;"); // Now try the same match with the global
flag. var reg = /[a-c]/g; result = src.match(reg); // The matches are in elements 0 through n. for (var index = 0; index &lt; result.length; index++) { document.write ("submatch " + index + ": " +
result[index]); document.write("&lt;br /&gt;"); }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="83092452-60cc-4218-b4ae-af9e3cb96c34.htm">exec Method (Regular Expression) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7f6b1073-8cbb-49ed-94b6-56833ba663c5.htm">RegExp Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="346aa83e-a045-47ea-acae-b42c7b121534.htm">Regular Expression Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="5f0e4765-df4d-4887-bd09-efe5e58251bf.htm">replace Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1cae0fbc-3319-4327-ba4e-d5fa2c4a9ba0.htm">search Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4f4b6e39-cb1a-4be9-a66f-7b846075580d.htm">test Method (Regular Expression) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Programming (Scripting)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Alternation and Subexpressions (Scripting)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Backreferences (Scripting)</span>
  </div>
</div>

