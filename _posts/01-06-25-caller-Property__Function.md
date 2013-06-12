---
title: caller Property (Function) (JavaScript)
---

### Introduction 

 Gets the function that invoked the current function.

### Syntax 

```
functionName .caller
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">functionName</span> object is the name of any executing function.
  </p>
  <p xmlns:util="util">
    The <b>caller</b> property is defined for a function only while that function is executing. If the function is called from the top level of a JavaScript program, <b>caller</b> contains
    <span sdata="langKeyword" value="null"><span class="keyword">null</span></span>.
  </p>
  <p xmlns:util="util">
    If the <b>caller</b> property is used in a string context, the result is the same as <span class="parameter" sdata="paramReference">functionName</span>.<b>toString</b>, that is, the decompiled
    text of the function is displayed.
  </p>
  <p xmlns:util="util">
    The following example illustrates the use of the <b>caller</b> property:
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
 function CallLevel(){    if (<span class=
"label">CallLevel.caller</span> == null)       return("CallLevel was called from the top level.");    else       return("CallLevel was called by another function."); }  document.write(CallLevel());  // Output: CallLevel was called from the top level. 
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
    <span sdata="link" xmlns:util="util"><a href="cc9cfd43-1305-41c8-ad67-545d20f4fafe.htm">function Statement (JavaScript)</a></span>
  </div>
</div>

