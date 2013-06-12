---
title: Bitwise AND Assignment Operator (&amp;=) (JavaScript)
---

### Introduction 

 Sets the result of a bitwise AND operation on the value of a variable and the value of an expression. The variable and the expression are treated as 32-bit integers.

### Syntax 

```
result &amp;= expression
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">result</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any variable.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any expression.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Using this operator is the same as specifying:
  </p>
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
 result = result &amp; expression 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    The <span sdata="link"><a href="a8c17a55-2599-4518-98d7-671699f4d5f3.htm">Bitwise AND Operator (&amp;) (JavaScript)</a></span> looks at the binary representation of the values of <span class=
    "parameter" sdata="paramReference">result</span> and <span class="parameter" sdata="paramReference">expression</span> and does a bitwise AND operation on them. The output of this operation
    behaves like this:
  </p>
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
 // 9 is 00000000000000000000000000001001 var expr1 = 9;  // 5 is 00000000000000000000000000000101 var expr2 = 5;    // 1 is 00000000000000000000000000000001 expr1 &amp;= expr2;  document.write(expr1); 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    Any time both of the expressions have a 1 in a digit, the result has a 1 in that digit. Otherwise, the result has a 0 in that digit.
  </p>
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
    <span sdata="link" xmlns:util="util"><a href="a8c17a55-2599-4518-98d7-671699f4d5f3.htm">Bitwise AND Operator (&amp;) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

