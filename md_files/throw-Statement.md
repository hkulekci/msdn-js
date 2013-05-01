## [throw Statement (JavaScript)](throw-Statement.html)

### Introduction 

 Generates an error condition that can be handled by a try...catch...finally statement.

### Syntax 

```
throw exception
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">exception</span> argument can be any expression.
  </p>
  <p xmlns:util="util">
    The following example throws an error inside a <span sdata="langKeyword" value="try"><span class="keyword">try</span></span> block, and it is caught in the <span sdata="langKeyword" value=
    "catch"><span class="keyword">catch</span></span> block.
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
 try {         throw new Error(200, "x equals zero"); } catch (e) {     document.write(e.message); }  // Output: x equals zero. 
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
    <span sdata="link" xmlns:util="util"><a href="b7a0a54e-dfaa-4e41-bf25-bcaa43e601fb.htm">try...catch...finally Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="0b27d6ec-3997-4e91-a6c0-5afbaf494db7.htm">Error Object (JavaScript)</a></span>
  </div>
</div>

