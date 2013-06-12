---
title: Bitwise AND Operator (&amp;) (JavaScript)
---

### Introduction 

 Performs a bitwise AND operation on two 32-bit expressions.

### Syntax 

```
result = expression1 &amp; 
expression2
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">result</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The result of the operation.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression2</span>
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
    The <span sdata="langKeyword" value="&amp;"><span class="keyword">&amp;</span></span> does a bitwise AND operation on the each of the bits of two 32-bit expressions. If both of the bits are 1,
    the result is 1. Otherwise, the result is 0.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Bit1
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Bit2
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            ANDed Value
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            0
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            0
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            0
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            1
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            1
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            1
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            1
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            0
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            0
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            0
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            1
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            0
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    The following examples show how to use the <span sdata="langKeyword" value="&amp;"><span class="keyword">&amp;</span></span> operator.
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
 // 9 is 00000000000000000000000000001001 var expr1 = 9;  // 5 is 00000000000000000000000000000101 var expr2 = 5;  // 1 is 00000000000000000000000000000001 var result = expr1 &amp; expr2;  document.write(result); // Output: 1 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util"></p>
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
    <span sdata="link" xmlns:util="util"><a href="e7e2eabb-4fc1-4fdc-9dd8-1e6d715371fa.htm">Bitwise AND Assignment Operator (&amp;=) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

