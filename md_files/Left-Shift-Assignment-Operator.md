---
title: Left Shift Assignment Operator (&lt;&lt;=) (JavaScript)
isChild: false
---

## Left Shift Assignment Operator (&lt;&lt;=) (JavaScript) {left_shift_assignment_operator_ltltequal_javascript_title}

### Introduction 

 Moves the specified number of bits to the left and assigns the result to result . The bits vacated by the operation are filled with 0.

### Syntax 

```
result &lt;&lt;= expression
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
        The number of bits to move.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Using the <b>&lt;&lt;=</b> operator is the same as specifying <span class="code">result = result &lt;&lt; expression</span>
  </p>
  <p xmlns:util="util">
    The following example shows how to use the <b>&lt;&lt;=</b> operator.
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
 // 14 is 00000000000000000000000000001110 var temp = 14; temp <span class="label">&lt;&lt;=</span> 2;  document.write(temp); // 56 is 00000000000000000000000000111000 Output: 56 
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

