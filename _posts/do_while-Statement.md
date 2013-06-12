---
title: do...while Statement (JavaScript)
isChild: false
---

## do...while Statement (JavaScript) {dowhile_statement_javascript_title}

### Introduction 

 Executes a statement block once, and then repeats execution of the loop until a condition expression evaluates to false .

### Syntax 

```
do { 
	statement } 
while (expression) ;
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statement</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The statement to be executed if <span class="parameter" sdata="paramReference">expression</span> is <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>.
        Can be a compound statement.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An expression that can be coerced to Boolean <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> or <span sdata="langKeyword" value="false"><span class=
        "keyword">false</span></span>. If <span class="parameter" sdata="paramReference">expression</span> is <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>, the loop
        is executed again. If <span class="parameter" sdata="paramReference">expression</span> is <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>, the loop is
        terminated.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Unlike the <span sdata="langKeyword" value="while"><span class="keyword">while</span></span> statement, a <span sdata="langKeyword" value="do...while"><span class=
    "keyword">do...while</span></span> loop is executed one time before the conditional expression is evaluated.
  </p>
  <p xmlns:util="util">
    On any line in a <span sdata="langKeyword" value="do&#8230;while"><span class="keyword">do&#8230;while</span></span> block, you can use the <span sdata="langKeyword" value="break"><span class=
    "keyword">break</span></span> statement to cause the program flow to exit the loop, or you can use the <span sdata="langKeyword" value="continue"><span class="keyword">continue</span></span>
    statement to go directly to the <span sdata="langKeyword" value="while"><span class="keyword">while</span></span> expression.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  In the following example, the statements in the <span sdata="langKeyword" value="do...while"><span class="keyword">do...while</span></span> loop continue to execute as long as the variable
  <span class="code">i</span> is less than 10.
</p>

```
var i = 0; do { document.write(i + " "); i++; } while (i &lt; 10); // Output: 0 1 2 3 4 5 6 7 8 9
```

<p xmlns:util="util">
  In the following example, the statements inside the loop are executed once even though the condition is not met.
</p>

```
var i = 10; do { document.write(i + " "); i++; } while (i &lt; 10); // Output: 10
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
    <span sdata="link" xmlns:util="util"><a href="bae0ec40-152e-43f3-969b-3696489ec5c4.htm">for Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1b51a0ce-89f7-4a69-88ed-017b47dc398f.htm">for...in Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d63777cf-0e1a-4555-8d3a-334381001f48.htm">while Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="019f898e-9e27-4be4-a22f-c5927c7fcae2.htm">Labeled Statement (JavaScript)</a></span>
  </div>
</div>

