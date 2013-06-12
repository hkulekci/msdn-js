---
title: lastIndexOf Method (String) (JavaScript)
isChild: false
---

## lastIndexOf Method (String) (JavaScript) {lastindexof_method_string_javascript_title}

### Introduction 

 Returns the last occurrence of a substring in the string.

### Syntax 

```
strObj .lastIndexOf(substring [, startindex ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">strObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">substring</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The substring to search for.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">startindex</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The index at which to begin searching. If omitted, the search begins at the end of the string.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>lastIndexOf</b> method returns an integer value indicating the beginning of the substring within the <span sdata="langKeyword" value="String"><span class="keyword">String</span></span>
    object. If the substring is not found, a -1 is returned.
  </p>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">startindex</span> is negative, <span class="parameter" sdata="paramReference">startindex</span> is treated as zero. If it is larger than the
    greatest character position index, it is treated as the largest possible index.
  </p>
  <p xmlns:util="util">
    Searching is performed starting at the last character in the string. Otherwise, this method is identical to <b>indexOf</b>.
  </p>
  <p xmlns:util="util">
    The following example illustrates the use of the <b>lastIndexOf</b> method.
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
 var str = "time, time";  var s = ""; s += "time is at position " + str.lastIndexOf("time"); s += "&lt;br /&gt;"; s += "abc is at position " + str.lastIndexOf("abc");  document.write(s);  // Output: // time is at position 6 // abc is at position -1 
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
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="a17372fa-669b-471b-9240-46927a265152.htm">indexOf Method (String) (JavaScript)</a></span>
  </div>
</div>

