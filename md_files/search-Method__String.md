## [search Method (String) (JavaScript)](search-Method__String.html)

### Introduction 

 Finds the first substring match in a regular expression search.

### Syntax 

```
stringObj .search(rgExp )
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
        Required. An instance of a <b>Regular Expression</b> object containing the regular expression pattern and applicable flags.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If a match is found, the <b>search</b> method returns an integer value that indicates the offset from the beginning of the string where the first match occurred. If no match is found, it returns
    -1.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You can also set the <span sdata="langKeyword" value="i"><span class="keyword">i</span></span> flag that causes the search to be case-insensitive.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>search</b> method.
</p>

```
var src = "is but a Dream within a dream"; var re = /dream/; var pos = src.search(re); document.write(pos); document.write("&lt;br/&gt;"); re = /dream/i; pos = src.search(re); document.write(pos); //
Output: // 24 // 9
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
    <span sdata="link" xmlns:util="util"><a href="eda9ad27-4f9b-4cb1-8345-a0ae85979ca0.htm">match Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="346aa83e-a045-47ea-acae-b42c7b121534.htm">Regular Expression Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="5f0e4765-df4d-4887-bd09-efe5e58251bf.htm">replace Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4f4b6e39-cb1a-4be9-a66f-7b846075580d.htm">test Method (Regular Expression) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Programming (Scripting)</span>
  </div>
</div>

