---
title: length Property (Array) (JavaScript)
isChild: false
---

## length Property (Array) (JavaScript) {length_property_array_javascript_title}

### Introduction 

 Gets or sets the length of the array. This is a number one higher than the highest element defined in an array.

### Syntax 

```
numVar = arrayObj .length
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numVar</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any number.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arrayObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any <b>Array</b> object.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    In JavaScript arrays are sparse, and the elements in an array do not have to be contiguous. The <b>length</b> property is not necessarily the number of elements in the array. For example, in the
    following array definition, <span class="code">my_array.length</span> contains 7, not 2:
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
 var my_array = new Array( ); my_array[0] = "Test"; my_array[6] = "Another Test"; 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    If you make the <b>length</b> property smaller than its previous value, the array is truncated, and any elements with array indexes equal to or greater than the new value of the <b>length</b>
    property are lost.
  </p>
  <p xmlns:util="util">
    If you make the length property larger than its previous value, the array is expanded, and any new elements created have the value <span sdata="langKeyword" value="undefined"><span class=
    "keyword">undefined</span></span>.
  </p>
  <p xmlns:util="util">
    The following example illustrates the use of the <b>length</b> property:
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
 var a; a = new Array(0,1,2,3,4); document.write(a.length);  // Output // 5 
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

