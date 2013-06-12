---
title: for Statement (JavaScript)
---

### Introduction 

 Executes a block of statements for as long as a specified condition is true.

### Syntax 

```
for ([initialization ]; 
[test ]; 
[increment ]) statement
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">initialization</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. An expression. This expression is executed only once, before the loop is executed.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">test</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A Boolean expression. If <span class="parameter" sdata="paramReference">test</span> is <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>, <span class=
        "parameter" sdata="paramReference">statement</span> is executed. If <span class="parameter" sdata="paramReference">test</span> if <span sdata="langKeyword" value="false"><span class=
        "keyword">false</span></span>, the loop is terminated.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">increment</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. An expression. The increment expression is executed at the end of every pass through the loop.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statement</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. One or more statements to be executed if <span class="parameter" sdata="paramReference">test</span> is <b>true</b>. Can be a compound statement.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You usually use a <span sdata="langKeyword" value="for"><span class="keyword">for</span></span> loop when the loop is to be executed a known number of times. A <span sdata="langKeyword" value=
    "for"><span class="keyword">for</span></span> loop is useful for iterating over arrays and for performing sequential processing.
  </p>
  <p xmlns:util="util">
    The test of a conditional expression occurs before the execution of the loop, so a <span sdata="langKeyword" value="for"><span class="keyword">for</span></span> statement executes zero or more
    times.
  </p>
  <p xmlns:util="util">
    On any line in a <span sdata="langKeyword" value="for"><span class="keyword">for</span></span> loop statement block, you can use the <span sdata="langKeyword" value="break"><span class=
    "keyword">break</span></span> statement to exit the loop, or you can use the <span sdata="langKeyword" value="continue"><span class="keyword">continue</span></span> statement to transfer control
    to the next iteration of the loop.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  In the following example, the <span sdata="langKeyword" value="for"><span class="keyword">for</span></span> statement executes the enclosed statements as follows:
</p>

```
// i is set to 0 at the start and is incremented by 1 at the // end of each iteration. // The loop terminates when i is not less than or equal to // 9 before a loop iteration. for (var i = 0; i &lt;=
9; i++) { document.write (i); document.write (" "); } // Output: 0 1 2 3 4 5 6 7 8 9
```

<p>
  First, the initial value of the variable <span class="code">i</span> is evaluated.
</p>

```
var j = 0; for (;;) { if (j &gt;= 5) { break; } j++; document.write (j + " "); } // Output: 1 2 3 4 5
```

<p>
  Then, as long as the value of <span class="code">i</span> is less than or equal to 9, the <span class="code">document.write</span> statements are executed and <span class="code">i</span> is
  reevaluated.
</p>

```
<p>
  Then, as long as the value of <span class="code">i</span> is less than or equal to 9, the <span class="code">document.write</span> statements are executed and <span class="code">i</span> is
  reevaluated.
</p>
```

<p>
  When <span class="code">i</span> is greater than 9, the condition becomes false and control is transferred outside the loop.
</p>

```
<p>
  When <span class="code">i</span> is greater than 9, the condition becomes false and control is transferred outside the loop.
</p>
```

<p xmlns:util="util">
  All of the expressions of the <span sdata="langKeyword" value="for"><span class="keyword">for</span></span> statement are optional. In the following example, the <span sdata="langKeyword" value=
  "for"><span class="keyword">for</span></span> statements create an infinite loop, and a <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement is used to exit
  the loop.
</p>

```
<p xmlns:util="util">
  All of the expressions of the <span sdata="langKeyword" value="for"><span class="keyword">for</span></span> statement are optional. In the following example, the <span sdata="langKeyword" value=
  "for"><span class="keyword">for</span></span> statements create an infinite loop, and a <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement is used to exit
  the loop.
</p>
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
    <span sdata="link" xmlns:util="util"><a href="1b51a0ce-89f7-4a69-88ed-017b47dc398f.htm">for...in Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d63777cf-0e1a-4555-8d3a-334381001f48.htm">while Statement (JavaScript)</a></span>
  </div>
</div>

