---
title: Bitwise Left Shift Operator (&lt;&lt;) (JavaScript)
isChild: false
---

## Bitwise Left Shift Operator (&lt;&lt;) (JavaScript) {bitwise_left_shift_operator_ltlt_javascript_title}

### Introduction 

 Left shifts the bits of an expression.

### Syntax 

```
result = expression1 &lt;&lt; 
expression2
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
      <i xmlns:util="util">expression1</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any expression.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">expression2</i>
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
    The <b>&lt;&lt;</b> operator shifts the bits of <i>expression1</i> left by the number of bits specified in <i>expression2</i>. For example:
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
 var temp temp = 14 <span class="label">&lt;&lt;</span> 2 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    The variable <i>temp</i> has a value of 56 because 14 (00001110 in binary) shifted left two bits equals 56 (00111000 in binary).
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
    <span sdata="link" xmlns:util="util"><a href="9f30ff46-48cc-4931-b260-edef31ff0076.htm">Left Shift Assignment Operator (&lt;&lt;=) (JavaScript)</a></span>
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

