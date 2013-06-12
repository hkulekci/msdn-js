---
title: String.fromCharCode Function (JavaScript)
---

### Introduction 

 Returns a string from a number of Unicode character values.

### Syntax 

```
String.fromCharCode([code1 [, code2 [, ...[, codeN ]]]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span sdata="langKeyword" value="String"><span class="keyword">String</span></span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">code1</span>, . . . , <span class="parameter" sdata="paramReference" xmlns:util="util">codeN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A series of Unicode character values to convert to a string. If no arguments are supplied, the result is the empty string.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You call this function on the <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object rather than on a string instance.
  </p>
  <p xmlns:util="util">
    The following example shows how to use this method:
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
 var test = String.fromCharCode(112, 108, 97, 105, 110); document.write(test);  // Output: plain 
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
    <span sdata="link" xmlns:util="util"><a href="5b0290a7-ee4d-4738-a909-c02ef64a2f1a.htm">charCodeAt Method (String) (JavaScript)</a></span>
  </div>
</div>

