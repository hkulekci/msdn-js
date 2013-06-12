---
title: parseInt Function (JavaScript)
isChild: false
---

## parseInt Function (JavaScript) {parseint_function_javascript_title}

### Introduction 

 Converts a string to an integer.

### Syntax 

```
parseInt(numString , [radix ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numString</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A string to convert into a number.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">radix</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A value between 2 and 36 that specifies the base of the number in <span class="parameter" sdata="paramReference">numString</span>. If this argument is not supplied, strings with a
        prefix of '0x' are considered hexadecimal. All other strings are considered decimal.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>parseInt</b> function returns an integer value equal to the number contained in <span class="parameter" sdata="paramReference">numString</span>. If no prefix of <span class="parameter"
    sdata="paramReference">numString</span> can be successfully parsed into an integer, <b>NaN</b> (not a number) is returned.
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
 parseInt("abc");     // Returns NaN. parseInt("12abc");   // Returns 12. 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    You can test for <b>NaN</b> using the <b>isNaN</b> function.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="81a40cad-9354-4e38-8ad0-83fc4257baee.htm">Global Object (JavaScript)</a></span>
  </p>
  <div class="alert">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th align="left">
          <img class="note" alt="Note" title="Note" src="../icons/alert_note.gif" /><b>Note</b>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Starting in Internet Explorer 9 standards mode, the <b>parseInt</b> function does not treat a string that has a prefix of '0' as an octal. When you are not using the <b>parseInt</b>
            function, however, strings with a prefix of '0' can still be interpreted as octals. See <span sdata="link">Data Types (JScript)</span> for information about octal integers.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="5af4eb29-72f6-484f-93bd-04ae1261f849.htm">isNaN Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="a7d87a69-1919-4623-be85-972e6376dd2d.htm">parseFloat Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="c555e38b-f451-4341-8fcd-4c8b02906a2c.htm">valueOf Method (Object) (JavaScript)</a></span>
  </div>
</div>

