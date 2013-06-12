---
title: valueOf Method (Array)
---

### Introduction 

 Returns the primitive value of the specified object.

### Syntax 

```
array .valueOf()
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    This method has no parameters.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns the array instance.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    In the following example, the instantiated array object is the same as the return value of this method.
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
 var arr = [1, 2, 3, 4]; var s = arr.valueOf();  if (arr === s) document.write("same"); else document.write("different");  // Output: // same  
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

