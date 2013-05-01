## [exec Method (Regular Expression) (JavaScript)](exec-Method__Regular-Expression.html)

### Introduction 

 Executes a search on a string using a regular expression pattern, and returns an array containing the results of that search.

### Syntax 

```
rgExp .exec(str )
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
        Required. The <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal on which to perform the search.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the <b>exec</b> method does not find a match, it returns <span sdata="langKeyword" value="null"><span class="keyword">null</span></span>. If it finds a match, <b>exec</b> returns an array, and
    the properties of the global <b>RegExp</b> object are updated to reflect the results of the match. Element zero of the array contains the entire match, while elements 1 &#8211; <i>n</i> contain
    any submatches that have occurred within the match. This behavior is identical to the behavior of the <b>match</b> method without the global flag (<b>g</b>) set.
  </p>
  <p xmlns:util="util">
    If the global flag is set for a regular expression, <b>exec</b> searches the string beginning at the position indicated by the value of <b>lastIndex</b>. If the global flag is not set,
    <b>exec</b> ignores the value of <b>lastIndex</b> and searches from the beginning of the string.
  </p>
  <p xmlns:util="util">
    The array returned by the <b>exec</b> method has three properties, <b>input</b>, <b>index</b> and <b>lastIndex.</b> The <b>input</b> property contains the entire searched string. The <b>index</b>
    property contains the position of the matched substring within the complete searched string. The <b>lastIndex</b> property contains the position following the last character in the match.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>exec</b> method:
</p>

```
function RegExpTest() { var ver = Number(ScriptEngineMajorVersion() + "." + ScriptEngineMinorVersion()) if (ver &lt; 5.5) { document.write("You need a newer version of JavaScript for this to work");
return; } var src = "The quick brown fox jumps over the lazy dog."; // Create regular expression pattern with a global flag. var re = /\w+/g; // Get the next word, starting at the position of
lastindex. var arr; while ((arr = re.exec(src)) != null) { // New line: document.write ("&lt;br /&gt;"); document.write (arr.index + "-" + arr.lastIndex + " "); document.write (arr[0]); } }
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
    <span sdata="link" xmlns:util="util"><a href="eda9ad27-4f9b-4cb1-8345-a0ae85979ca0.htm">match Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7f6b1073-8cbb-49ed-94b6-56833ba663c5.htm">RegExp Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
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
</div>

