---
title: Right Shift Assignment Operator (&gt;&gt;=) (JavaScript)
isChild: false
---

## Right Shift Assignment Operator (&gt;&gt;=) (JavaScript) {right_shift_assignment_operator_gtgtequal_javascript_title}

### Introduction 

 Right shifts the value of a variable by the number of bits specified in the value of an expression, maintaining the sign, and assigns the result to the variable.

### Syntax 

```
result &gt;&gt;= expression
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">result</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any variable.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">expression</i>
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
    Using the <b>&gt;&gt;=</b> operator is exactly the same as specifying:
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
 result = result &gt;&gt; expression 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    The <b>&gt;&gt;=</b> operator shifts the bits of <i>result</i> right by the number of bits specified in <i>expression</i>. The sign bit of <i>result</i> is used to fill the digits from the left.
    Digits shifted off the right are discarded. For example, after the following code is evaluated, <i>temp</i> has a value of -4: 14 (11110010 in binary) shifted right two bits equals -4 (11111100
    in binary).
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
 var temp temp = -14 temp <span class="label">&gt;&gt;=</span> 2 
</pre>
        </td>
      </tr>
    </table>
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
    <span sdata="link" xmlns:util="util"><a href="18148596-7b86-4add-aeef-106991c69435.htm">Bitwise Left Shift Operator (&lt;&lt;) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="89dc57e0-0b0d-49a4-a8ed-56d8bb20f3e3.htm">Bitwise Right Shift Operator (&gt;&gt;) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="df48bdfc-8741-46ab-b681-449da57ac95c.htm">Unsigned Right Shift Operator (&gt;&gt;&gt;) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

