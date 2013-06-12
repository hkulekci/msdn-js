---
title: parseFloat Function (JavaScript)
isChild: false
---

## parseFloat Function (JavaScript) {parsefloat_function_javascript_title}

### Introduction 

 Converts a string to a floating-point number.

### Syntax 

```
parseFloat(numString )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">numString</span> argument is a string that contains a floating-point number.
  </p>
  <p xmlns:util="util">
    The <b>parseFloat</b> function returns a numerical value equal to the number contained in <span class="parameter" sdata="paramReference">numString</span>. If no prefix of <span class="parameter"
    sdata="paramReference">numString</span> can be successfully parsed into a floating-point number, <b>NaN</b> (not a number) is returned.
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
 parseFloat("abc")      // Returns NaN. parseFloat("1.2abc")   // Returns 1.2. 
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
    <span sdata="link" xmlns:util="util"><a href="e86471af-2a0e-4359-83af-f1ac81e51421.htm">parseInt Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

