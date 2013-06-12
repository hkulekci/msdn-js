---
title: while Statement (JavaScript)
---

### Introduction 

 Executes a statement or series of statements until a specified condition is false .

### Syntax 

```
while (expression ) { 
	statements }
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A Boolean expression that is checked before each iteration of the loop. If <span class="parameter" sdata="paramReference">expression</span> is <span sdata="langKeyword" value=
        "true"><span class="keyword">true</span></span>, the loop is executed. If <span class="parameter" sdata="paramReference">expression</span> is <span sdata="langKeyword" value=
        "false"><span class="keyword">false</span></span>, the loop is terminated.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statements</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. One or more statements to be executed if <span class="parameter" sdata="paramReference">expression</span> is <span sdata="langKeyword" value="true"><span class=
        "keyword">true</span></span>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="while"><span class="keyword">while</span></span> statement checks <span class="parameter" sdata="paramReference">expression</span> before a loop is first
    executed. If <span class="parameter" sdata="paramReference">expression</span> is <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> at this time, the loop is never
    executed.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="while"><span class="keyword">while</span></span> statement.
</p>

```
var i = 0; var j = 10; while (i &lt; 100) { if (i == j) break; i++; } document.write(i); // Output: 10
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
    <span sdata="link" xmlns:util="util"><a href="5be0f2a8-5fe7-4a6c-89af-ca20a925ce87.htm">break Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="f8a30d9f-e2de-4e1f-8668-4e4cf95f7df9.htm">continue Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8b7782ba-fbad-48cd-9639-193566da6ae5.htm">do...while Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="bae0ec40-152e-43f3-969b-3696489ec5c4.htm">for Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1b51a0ce-89f7-4a69-88ed-017b47dc398f.htm">for...in Statement (JavaScript)</a></span>
  </div>
</div>

