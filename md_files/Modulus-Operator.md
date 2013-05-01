## [Modulus Operator (JavaScript)](Modulus-Operator.html)

### Introduction 

 Divides the value of one expression by the value of another, and returns the remainder.

### Syntax 

```
result = number1 % number2
```

#### Arguments 

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
      <span class="parameter" sdata="paramReference" xmlns:util="util">number1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any numeric expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">number2</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any numeric expression.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The modulus, or remainder, operator divides <span class="parameter" sdata="paramReference">number1</span> by <span class="parameter" sdata="paramReference">number2</span>and returns only the
    remainder as <span class="parameter" sdata="paramReference">result</span>. The sign of <span class="parameter" sdata="paramReference">result</span> is the same as the sign of <span class=
    "parameter" sdata="paramReference">number1</span>. The value of <span class="parameter" sdata="paramReference">result</span> is between 0 and the absolute value of <span class="parameter" sdata=
    "paramReference">number2</span>.
  </p>
  <p xmlns:util="util">
    The following code shows how to use the modulus operator.
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          &nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 var modResult = 19 % 6.7; document.write(modResult);  // Output: 5.6 
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
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

