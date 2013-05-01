## [break Statement (JavaScript)](break-Statement.html)

### Introduction 

 Terminates the current loop, or if in conjunction with a label , terminates the associated statement.

### Syntax 

```
break [label ];
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The optional <span class="parameter" sdata="paramReference">label</span> argument specifies the label of the statement you are breaking from.
  </p>
  <p xmlns:util="util">
    You typically use the <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement in <span sdata="langKeyword" value="switch"><span class=
    "keyword">switch</span></span> statements and in <span sdata="langKeyword" value="while"><span class="keyword">while</span></span>, <span sdata="langKeyword" value="for"><span class=
    "keyword">for</span></span>, <span sdata="langKeyword" value="for...in"><span class="keyword">for...in</span></span>, or <span sdata="langKeyword" value="do...while"><span class=
    "keyword">do...while</span></span> loops. You most commonly use the <span class="parameter" sdata="paramReference">label</span> argument in <span sdata="langKeyword" value="switch"><span class=
    "keyword">switch</span></span> statements, but it can be used in any statement, whether simple or compound.
  </p>
  <p xmlns:util="util">
    Executing the <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement exits from the current loop or statement, and begins script execution with the statement
    immediately following.
  </p>
</div>

#### Examples 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <div id="sectionSection1" class="seeAlsoNoToggleSection">
    <p xmlns:util="util">
      In this example, the counter is set up to count from 1 to 99; however, the <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement terminates the loop after
      14 counts.
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
 for (var i = 1; i &lt; 100; i++) {     if (i == 15) {         break;     }     document.write (i);     document.write (" "); }  // Output: 1234567891011121314 
</pre>
          </td>
        </tr>
      </table>
    </div>
  </div>
  <div id="sectionSection3" class="seeAlsoNoToggleSection">
    <p xmlns:util="util">
      In the following code, the <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement refers to the <span sdata="langKeyword" value="for"><span class=
      "keyword">for</span></span> loop that is preceded by the <span class="code">Inner:</span> statement. When <span class="code">j</span> is equal to 24, the <span sdata="langKeyword" value=
      "break"><span class="keyword">break</span></span> statement causes the program flow to exit that loop. The numbers 21 through 23 print on each line.
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
 Outer: for (var i = 1; i &lt;= 10; i++) {     document.write ("&lt;br /&gt;");     document.write ("i: " + i);     document.write (" j: "); Inner:     for (var j = 21; j &lt;= 30; j++) {         if (j == 24) {             break Inner;         }         document.write (j + " ");     } }  // Output:  // i: 1 j: 21 22 23  // i: 2 j: 21 22 23  // i: 3 j: 21 22 23  // i: 4 j: 21 22 23  // i: 5 j: 21 22 23  // i: 6 j: 21 22 23  // i: 7 j: 21 22 23  // i: 8 j: 21 22 23  // i: 9 j: 21 22 23  // i: 10 j: 21 22 23 
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
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="019f898e-9e27-4be4-a22f-c5927c7fcae2.htm">Labeled Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d63777cf-0e1a-4555-8d3a-334381001f48.htm">while Statement (JavaScript)</a></span>
  </div>
</div>

