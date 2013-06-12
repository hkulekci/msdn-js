---
title: continue Statement (JavaScript)
isChild: false
---

## continue Statement (JavaScript) {continue_statement_javascript_title}

### Introduction 

 Stops the current iteration of a loop, and starts a new iteration.

### Syntax 

```
continue [label ];
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The optional <span class="parameter" sdata="paramReference">label</span> argument specifies the statement to which <span sdata="langKeyword" value="continue"><span class=
    "keyword">continue</span></span> applies.
  </p>
  <p xmlns:util="util">
    You can use the <span sdata="langKeyword" value="continue"><span class="keyword">continue</span></span> statement only inside a <span sdata="langKeyword" value="while"><span class=
    "keyword">while</span></span>, <span sdata="langKeyword" value="do...while"><span class="keyword">do...while</span></span>, <b>for</b>, or <span sdata="langKeyword" value="for...in"><span class=
    "keyword">for...in</span></span> loop. Executing the <span sdata="langKeyword" value="continue"><span class="keyword">continue</span></span> statement stops the current iteration of the loop and
    continues program flow with the beginning of the loop. This has the following effects on the different types of loops:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        <span sdata="langKeyword" value="while"><span class="keyword">while</span></span> and <span sdata="langKeyword" value="do...while"><span class="keyword">do...while</span></span> loops test
        their condition, and if true, execute the loop again.
      </p>
    </li>
    <li>
      <p>
        <span sdata="langKeyword" value="for"><span class="keyword">for</span></span> loops execute their increment expression, and if the test expression is true, execute the loop again.
      </p>
    </li>
    <li>
      <p>
        <span sdata="langKeyword" value="for...in"><span class="keyword">for...in</span></span> loops proceed to the next field of the specified variable and execute the loop again.
      </p>
    </li>
  </ul>
</div>

#### Examples 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <div id="sectionSection1" class="seeAlsoNoToggleSection">
    <p xmlns:util="util">
      In this example, a loop iterates from 1 through 9. The statements between <span sdata="langKeyword" value="continue"><span class="keyword">continue</span></span> and the end of the <span sdata=
      "langKeyword" value="for"><span class="keyword">for</span></span> body are skipped because of the use of the <span sdata="langKeyword" value="continue"><span class=
      "keyword">continue</span></span> statement together with the expression <span class="code">(i &lt; 5)</span>.
    </p>
  </div>
  <div id="sectionSection2" class="seeAlsoNoToggleSection">
    <div class="code">
      <table width="100%" cellspacing="0" cellpadding="0">
        <tr>
          <th>
            JavaScript&nbsp;
          </th>
          <th>
            <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
            "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
          </th>
        </tr>
        <tr>
          <td colspan="2">
            <pre>
 for (var i = 1; i &lt; 10; i++) {     if (i &lt; 5) {         continue;     }     document.write (i);     document.write (" "); }  // Output: 5 6 7 8 9 
</pre>
          </td>
        </tr>
      </table>
    </div>
  </div>
  <div id="sectionSection3" class="seeAlsoNoToggleSection">
    <p xmlns:util="util">
      In the following code, the <span sdata="langKeyword" value="continue"><span class="keyword">continue</span></span> statement refers to the <span sdata="langKeyword" value="for"><span class=
      "keyword">for</span></span> loop that is preceded by the <span class="code">Inner:</span> label. When <span class="code">j</span> is 24, the <span sdata="langKeyword" value=
      "continue"><span class="keyword">continue</span></span> statement causes that <span sdata="langKeyword" value="for"><span class="keyword">for</span></span> loop to go to the next iteration. The
      numbers 21 through 23 and 25 through 30 print on each line.
    </p>
  </div>
  <div id="sectionSection4" class="seeAlsoNoToggleSection">
    <div class="code">
      <table width="100%" cellspacing="0" cellpadding="0">
        <tr>
          <th>
            JavaScript&nbsp;
          </th>
          <th>
            <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
            "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
          </th>
        </tr>
        <tr>
          <td colspan="2">
            <pre>
 Outer: for (var i = 1; i &lt;= 10; i++) {     document.write ("&lt;br /&gt;");     document.write ("i: " + i);     document.write (" j: ");     Inner:     for (var j = 21; j &lt;= 30; j++) {         if (j == 24) {              continue Inner;         }         document.write (j + " ");     } }  //Output: //i: 1 j: 21 22 23 25 26 27 28 29 30  //i: 2 j: 21 22 23 25 26 27 28 29 30  //i: 3 j: 21 22 23 25 26 27 28 29 30  //i: 4 j: 21 22 23 25 26 27 28 29 30  //i: 5 j: 21 22 23 25 26 27 28 29 30  //i: 6 j: 21 22 23 25 26 27 28 29 30  //i: 7 j: 21 22 23 25 26 27 28 29 30  //i: 8 j: 21 22 23 25 26 27 28 29 30  //i: 9 j: 21 22 23 25 26 27 28 29 30  //i: 10 j: 21 22 23 25 26 27 28 29 30 
</pre>
          </td>
        </tr>
      </table>
    </div>
  </div>
</div>

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
    <span sdata="link" xmlns:util="util"><a href="8b7782ba-fbad-48cd-9639-193566da6ae5.htm">do...while Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="bae0ec40-152e-43f3-969b-3696489ec5c4.htm">for Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1b51a0ce-89f7-4a69-88ed-017b47dc398f.htm">for...in Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="019f898e-9e27-4be4-a22f-c5927c7fcae2.htm">Labeled Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d63777cf-0e1a-4555-8d3a-334381001f48.htm">while Statement (JavaScript)</a></span>
  </div>
</div>

