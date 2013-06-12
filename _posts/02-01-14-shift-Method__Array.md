---
title: shift Method (Array) (JavaScript)
---

### Introduction 

 Removes the first element from an array and returns it.

### Syntax 

```
arrayObj .shift( )
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">arrayObj</span> reference is an <b>Array</b> object.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns the element removed from the array.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The following example illustrates the use of the <span sdata="langKeyword" value="shift"><span class="keyword">shift</span></span> method.
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
 var arr = new Array(10, 11, 12); while (arr.length &gt; 0)     {     var i = arr.shift();     document.write (i.toString() + " ");     }  // Output:  // 10 11 12 
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
    <span sdata="link" xmlns:util="util"><a href="8c6a39ed-bab3-4ca4-9350-571a9427ec94.htm">unshift Method (Array) (JavaScript)</a></span>
  </div>
</div>

